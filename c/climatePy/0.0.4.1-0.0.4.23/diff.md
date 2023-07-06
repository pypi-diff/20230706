# Comparing `tmp/climatePy-0.0.4.1.tar.gz` & `tmp/climatePy-0.0.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.0.4.1.tar", last modified: Thu Jun 29 14:45:02 2023, max compression
+gzip compressed data, was "climatePy-0.0.4.23.tar", last modified: Thu Jul  6 20:07:50 2023, max compression
```

## Comparing `climatePy-0.0.4.1.tar` & `climatePy-0.0.4.23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.549918 climatePy-0.0.4.1/
--rw-rw-rw-   0        0        0     1108 2023-06-23 23:24:45.000000 climatePy-0.0.4.1/LICENSE
--rw-rw-rw-   0        0        0     5557 2023-06-29 14:45:02.548919 climatePy-0.0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5139 2023-06-28 16:33:45.000000 climatePy-0.0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.461919 climatePy-0.0.4.1/climatePy/
--rw-rw-rw-   0        0        0     1848 2023-06-29 14:34:25.000000 climatePy-0.0.4.1/climatePy/__init__.py
--rw-rw-rw-   0        0        0     8861 2023-06-29 14:21:36.000000 climatePy-0.0.4.1/climatePy/_climatepy_filter.py
--rw-rw-rw-   0        0        0    60987 2023-06-29 14:21:29.000000 climatePy-0.0.4.1/climatePy/_dap.py
--rw-rw-rw-   0        0        0     3623 2023-06-29 14:21:30.000000 climatePy-0.0.4.1/climatePy/_netrc_utils.py
--rw-rw-rw-   0        0        0    33802 2023-06-29 14:34:46.000000 climatePy-0.0.4.1/climatePy/_shortcuts.py
--rw-rw-rw-   0        0        0    27503 2023-06-29 14:21:34.000000 climatePy-0.0.4.1/climatePy/_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.476918 climatePy-0.0.4.1/climatePy/data/
--rw-rw-rw-   0        0        0 45897655 2023-03-04 16:05:07.000000 climatePy-0.0.4.1/climatePy/data/catalog.csv
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.475919 climatePy-0.0.4.1/climatePy.egg-info/
--rw-rw-rw-   0        0        0     5557 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-29 14:45:02.000000 climatePy-0.0.4.1/climatePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:45:02.549918 climatePy-0.0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-06-29 14:43:59.000000 climatePy-0.0.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:02.547919 climatePy-0.0.4.1/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 21:55:17.000000 climatePy-0.0.4.1/tests/__init__.py
--rw-rw-rw-   0        0        0    44952 2023-06-29 14:43:15.000000 climatePy-0.0.4.1/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     3253 2023-06-29 14:43:13.000000 climatePy-0.0.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.340048 climatePy-0.0.4.23/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20981 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59354 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32737 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26691 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.340048 climatePy-0.0.4.23/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.340048 climatePy-0.0.4.23/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 20:07:50.000000 climatePy-0.0.4.23/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:50.384048 climatePy-0.0.4.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43848 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 20:07:41.000000 climatePy-0.0.4.23/tests/test_utils.py
```

### Comparing `climatePy-0.0.4.1/LICENSE` & `climatePy-0.0.4.23/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Angus Watters, Mike J. Johnson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Angus Watters, Mike J. Johnson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `climatePy-0.0.4.1/PKG-INFO` & `climatePy-0.0.4.23/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,175 +1,184 @@
-Metadata-Version: 2.1
-Name: climatePy
-Version: 0.0.4.1
-Summary: A Python package for getting point and gridded climate data by AOI
-Author: Angus Watters, Mike Johnson
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# [**climatePy**](https://github.com/LynkerIntel/climatePy)
-
-<!-- badges: start -->
-
-[![stage](https://img.shields.io/badge/stage-dev-orange)](#)
-[![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
-[![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
-
-<!-- badges: end -->
-
-## Description
-
-A Python ðŸ“¦ for getting point and gridded climate data by AOI. `climatePy` is the Python version of the [`climateR`](https://github.com/mikejohnson51/climateR) R package, providing all of the same functionality but in Python.
-
-As its stated in the [climateR README](https://github.com/mikejohnson51/climateR#climater):
-climatePy simplifies the steps needed to get climate data into Python. At its core it provides three main things:
-
-1. A climate catalog of over 100,000k datasets from over 2,000 data providers/archives. See (`params()`)
-
-2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
-
-3. A set of shortcuts that implement these methods for a core set of selected catalog elements
-
-<br>
-
----
-
-- [climatePy PyPI](https://pypi.org/project/climatePy/)
-- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
-
----
-
-## Table of Contents (Optional)
-
-- [Installation](#installation)
-- [Usage](#usage)
-- [Credits](#credits)
-- [License](#license)
-- [How to Contribute](#how-to-contribute)
-
-<br>
-
-## Installation
-
-`climatePy` can be downloaded from PyPI via `pip` like so:
-
-``` 
-pip install climatePy
-```
-**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
-
-<br>
-
-## Usage
-
-### Loading climate catalog
-
-```python
-import geopandas as gpd
-import matplotlib.pyplot as plt
-from climatePy import params
-
-# load climate catalog
-catalog = params()
-
-# load example AOI data
-AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
-```
-<br>
-
-### Using `climatepy_filter()`:
-
-The `climatepy_filter()` is one of the core functions of `climatePy` and is used to do the first round of filtering on the base climate catalog.
-
-Here we filter down our climate catalog to TerraClim precipitation data for San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-raw = climatePy.climatepy_filter(
-        id        = "terraclim", 
-        AOI       = AOI, 
-        varname   = "ppt"
-        )
-```
-
-| id  | asset | varname    |
-|-------|-----|---------|
-| gridmet | agg_terraclimate_ppt_1958_CurrentYear_GLOBE  | ppt   |
-
-### AOI
-![San Luis Obispo County county](assets/images/san_luis_obispo_county_polygon.png)
-
-<br>
-
-### Getting climate data in AOI
-
-Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-prcp = shortcuts.getTerraClim(
-    AOI       = AOI,
-    varname   = "ppt",
-    startDate = "2018-01-01",
-    endDate   = "2018-01-01"
-    )
-```
-![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
-
-<br>
-<br>
-
-### Get data within a date range
-
-We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-prcp = shortcuts.getTerraClim(
-    AOI       = AOI,
-    varname   = "ppt",
-    startDate = "2018-01-01",
-    endDate   = "2018-12-01"
-    )
-```
-![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
-
-<br>
-<br>
-
-## Credits
-
-Credit to [Mike J Johnson](https://github.com/mikejohnson51) and the other contributors to the original [`climateR`](https://github.com/mikejohnson51/climateR) package listed below:
-- [Max Joseph](https://github.com/mbjoseph)
-- [Eric R. Scott](https://github.com/Aariq)
-- [James Tsakalos](https://github.com/jamestsakalos)
-
-<br>
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Angus Watters, Mike J. Johnson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
----
-
-<br>
-
-## How to Contribute
-If you would like to contribute, submit a PR and we will get to as soon as we can!
-If you have any issues please open an issue on GitHub. For any questions, feel free to ask [@anguswg-ucsb](https://github.com/anguswg-ucsb) or [@mikejohnson51](https://github.com/mikejohnson51), or simply create an issue on GitHub.
+# [**climatePy**](https://github.com/LynkerIntel/climatePy)
+
+<!-- badges: start -->
+
+[![stage](https://img.shields.io/badge/stage-dev-orange)](#)
+[![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
+[![License:
+MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+
+<!-- badges: end -->
+
+## Description
+
+A Python 📦 for getting point and gridded climate data by AOI. `climatePy` is the Python version of the [`climateR`](https://github.com/mikejohnson51/climateR) R package, providing all of the same functionality but in Python.
+
+As its stated in the [climateR README](https://github.com/mikejohnson51/climateR#climater):
+climatePy simplifies the steps needed to get climate data into Python. At its core it provides three main things:
+
+1. A climate catalog of over 100,000k datasets from over 2,000 data providers/archives. See (`params()`)
+
+2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
+
+3. A set of shortcuts that implement these methods for a core set of selected catalog elements
+
+<br>
+
+---
+
+- [climatePy PyPI](https://pypi.org/project/climatePy/)
+- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
+
+---
+
+## Table of Contents (Optional)
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Credits](#credits)
+- [License](#license)
+- [How to Contribute](#how-to-contribute)
+
+<br>
+
+## Installation
+
+`climatePy` can be downloaded from PyPI via `pip` like so:
+
+``` 
+pip install climatePy
+```
+**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
+
+<br>
+
+## Usage
+
+### Loading climate catalog
+
+```python
+import geopandas as gpd
+import matplotlib.pyplot as plt
+from climatePy import params
+
+# load climate catalog
+catalog = params()
+
+# load example AOI data
+AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
+```
+<br>
+
+### Using `climatepy_filter()`:
+
+The `climatepy_filter()` is one of the core functions of `climatePy` and is used to do the first round of filtering on the base climate catalog.
+
+Here we filter down our climate catalog to TerraClim precipitation data for San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+raw = climatePy.climatepy_filter(
+        id        = "terraclim", 
+        AOI       = AOI, 
+        varname   = "ppt"
+        )
+```
+
+| id  | asset | varname    |
+|-------|-----|---------|
+| gridmet | agg_terraclimate_ppt_1958_CurrentYear_GLOBE  | ppt   |
+
+### AOI
+![San Luis Obispo County county](assets/images/san_luis_obispo_county_polygon.png)
+
+<br>
+
+### Getting climate data in AOI
+
+Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+prcp = shortcuts.getTerraClim(
+    AOI       = AOI,
+    varname   = "ppt",
+    startDate = "2018-01-01",
+    endDate   = "2018-01-01"
+    )
+```
+![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
+
+<br>
+<br>
+
+### Get data within a date range
+
+We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+prcp = shortcuts.getTerraClim(
+    AOI       = AOI,
+    varname   = "ppt",
+    startDate = "2018-01-01",
+    endDate   = "2018-12-01"
+    )
+```
+![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
+
+<br>
+
+### Data from known bounding coordinates
+
+`climatePy` offers support for `shapely` bounding boxes. Here we are requesting wind velocity data for the four corners region of the USA by bounding coordinates.
+
+```python
+from shapely.geometry import box
+
+bbox = box(-112, 34, -105, 39)
+
+bbox = gpd.GeoDataFrame(geometry=[bbox], crs ='EPSG:4326')
+
+vs = climatePy.getGridMET(
+       AOI       = bbox, 
+       varname   = "vs",
+       startDate = "2018-09-01"
+       )
+```
+![Daily Wind Velocity Four Corners, USA](assets/images/four_corners_gridmet.png)
+
+<br>
+<br>
+
+## Credits
+
+Credit to [Mike J Johnson](https://github.com/mikejohnson51) and the other contributors to the original [`climateR`](https://github.com/mikejohnson51/climateR) package listed below:
+- [Max Joseph](https://github.com/mbjoseph)
+- [Eric R. Scott](https://github.com/Aariq)
+- [James Tsakalos](https://github.com/jamestsakalos)
+
+<br>
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Angus Watters, Mike J. Johnson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+---
+
+<br>
+
+## How to Contribute
+If you would like to contribute, submit a PR and we will get to as soon as we can!
+If you have any issues please open an issue on GitHub. For any questions, feel free to ask [@anguswg-ucsb](https://github.com/anguswg-ucsb) or [@mikejohnson51](https://github.com/mikejohnson51), or simply create an issue on GitHub.
```

### Comparing `climatePy-0.0.4.1/README.md` & `climatePy-0.0.4.23/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,163 +1,196 @@
-# [**climatePy**](https://github.com/LynkerIntel/climatePy)
-
-<!-- badges: start -->
-
-[![stage](https://img.shields.io/badge/stage-dev-orange)](#)
-[![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
-[![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
-
-<!-- badges: end -->
-
-## Description
-
-A Python 📦 for getting point and gridded climate data by AOI. `climatePy` is the Python version of the [`climateR`](https://github.com/mikejohnson51/climateR) R package, providing all of the same functionality but in Python.
-
-As its stated in the [climateR README](https://github.com/mikejohnson51/climateR#climater):
-climatePy simplifies the steps needed to get climate data into Python. At its core it provides three main things:
-
-1. A climate catalog of over 100,000k datasets from over 2,000 data providers/archives. See (`params()`)
-
-2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
-
-3. A set of shortcuts that implement these methods for a core set of selected catalog elements
-
-<br>
-
----
-
-- [climatePy PyPI](https://pypi.org/project/climatePy/)
-- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
-
----
-
-## Table of Contents (Optional)
-
-- [Installation](#installation)
-- [Usage](#usage)
-- [Credits](#credits)
-- [License](#license)
-- [How to Contribute](#how-to-contribute)
-
-<br>
-
-## Installation
-
-`climatePy` can be downloaded from PyPI via `pip` like so:
-
-``` 
-pip install climatePy
-```
-**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
-
-<br>
-
-## Usage
-
-### Loading climate catalog
-
-```python
-import geopandas as gpd
-import matplotlib.pyplot as plt
-from climatePy import params
-
-# load climate catalog
-catalog = params()
-
-# load example AOI data
-AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
-```
-<br>
-
-### Using `climatepy_filter()`:
-
-The `climatepy_filter()` is one of the core functions of `climatePy` and is used to do the first round of filtering on the base climate catalog.
-
-Here we filter down our climate catalog to TerraClim precipitation data for San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-raw = climatePy.climatepy_filter(
-        id        = "terraclim", 
-        AOI       = AOI, 
-        varname   = "ppt"
-        )
-```
-
-| id  | asset | varname    |
-|-------|-----|---------|
-| gridmet | agg_terraclimate_ppt_1958_CurrentYear_GLOBE  | ppt   |
-
-### AOI
-![San Luis Obispo County county](assets/images/san_luis_obispo_county_polygon.png)
-
-<br>
-
-### Getting climate data in AOI
-
-Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-prcp = shortcuts.getTerraClim(
-    AOI       = AOI,
-    varname   = "ppt",
-    startDate = "2018-01-01",
-    endDate   = "2018-01-01"
-    )
-```
-![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
-
-<br>
-<br>
-
-### Get data within a date range
-
-We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-prcp = shortcuts.getTerraClim(
-    AOI       = AOI,
-    varname   = "ppt",
-    startDate = "2018-01-01",
-    endDate   = "2018-12-01"
-    )
-```
-![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
-
-<br>
-<br>
-
-## Credits
-
-Credit to [Mike J Johnson](https://github.com/mikejohnson51) and the other contributors to the original [`climateR`](https://github.com/mikejohnson51/climateR) package listed below:
-- [Max Joseph](https://github.com/mbjoseph)
-- [Eric R. Scott](https://github.com/Aariq)
-- [James Tsakalos](https://github.com/jamestsakalos)
-
-<br>
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Angus Watters, Mike J. Johnson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
----
-
-<br>
-
-## How to Contribute
-If you would like to contribute, submit a PR and we will get to as soon as we can!
-If you have any issues please open an issue on GitHub. For any questions, feel free to ask [@anguswg-ucsb](https://github.com/anguswg-ucsb) or [@mikejohnson51](https://github.com/mikejohnson51), or simply create an issue on GitHub.
+Metadata-Version: 2.1
+Name: climatePy
+Version: 0.0.4.23
+Summary: A Python package for getting point and gridded climate data by AOI
+Author: Angus Watters, Mike Johnson
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [**climatePy**](https://github.com/LynkerIntel/climatePy)
+
+<!-- badges: start -->
+
+[![stage](https://img.shields.io/badge/stage-dev-orange)](#)
+[![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
+[![License:
+MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+
+<!-- badges: end -->
+
+## Description
+
+A Python 📦 for getting point and gridded climate data by AOI. `climatePy` is the Python version of the [`climateR`](https://github.com/mikejohnson51/climateR) R package, providing all of the same functionality but in Python.
+
+As its stated in the [climateR README](https://github.com/mikejohnson51/climateR#climater):
+climatePy simplifies the steps needed to get climate data into Python. At its core it provides three main things:
+
+1. A climate catalog of over 100,000k datasets from over 2,000 data providers/archives. See (`params()`)
+
+2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
+
+3. A set of shortcuts that implement these methods for a core set of selected catalog elements
+
+<br>
+
+---
+
+- [climatePy PyPI](https://pypi.org/project/climatePy/)
+- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
+
+---
+
+## Table of Contents (Optional)
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Credits](#credits)
+- [License](#license)
+- [How to Contribute](#how-to-contribute)
+
+<br>
+
+## Installation
+
+`climatePy` can be downloaded from PyPI via `pip` like so:
+
+``` 
+pip install climatePy
+```
+**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
+
+<br>
+
+## Usage
+
+### Loading climate catalog
+
+```python
+import geopandas as gpd
+import matplotlib.pyplot as plt
+from climatePy import params
+
+# load climate catalog
+catalog = params()
+
+# load example AOI data
+AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
+```
+<br>
+
+### Using `climatepy_filter()`:
+
+The `climatepy_filter()` is one of the core functions of `climatePy` and is used to do the first round of filtering on the base climate catalog.
+
+Here we filter down our climate catalog to TerraClim precipitation data for San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+raw = climatePy.climatepy_filter(
+        id        = "terraclim", 
+        AOI       = AOI, 
+        varname   = "ppt"
+        )
+```
+
+| id  | asset | varname    |
+|-------|-----|---------|
+| gridmet | agg_terraclimate_ppt_1958_CurrentYear_GLOBE  | ppt   |
+
+### AOI
+![San Luis Obispo County county](assets/images/san_luis_obispo_county_polygon.png)
+
+<br>
+
+### Getting climate data in AOI
+
+Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+prcp = shortcuts.getTerraClim(
+    AOI       = AOI,
+    varname   = "ppt",
+    startDate = "2018-01-01",
+    endDate   = "2018-01-01"
+    )
+```
+![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
+
+<br>
+<br>
+
+### Get data within a date range
+
+We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+prcp = shortcuts.getTerraClim(
+    AOI       = AOI,
+    varname   = "ppt",
+    startDate = "2018-01-01",
+    endDate   = "2018-12-01"
+    )
+```
+![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
+
+<br>
+
+### Data from known bounding coordinates
+
+`climatePy` offers support for `shapely` bounding boxes. Here we are requesting wind velocity data for the four corners region of the USA by bounding coordinates.
+
+```python
+from shapely.geometry import box
+
+bbox = box(-112, 34, -105, 39)
+
+bbox = gpd.GeoDataFrame(geometry=[bbox], crs ='EPSG:4326')
+
+vs = climatePy.getGridMET(
+       AOI       = bbox, 
+       varname   = "vs",
+       startDate = "2018-09-01"
+       )
+```
+![Daily Wind Velocity Four Corners, USA](assets/images/four_corners_gridmet.png)
+
+<br>
+<br>
+
+## Credits
+
+Credit to [Mike J Johnson](https://github.com/mikejohnson51) and the other contributors to the original [`climateR`](https://github.com/mikejohnson51/climateR) package listed below:
+- [Max Joseph](https://github.com/mbjoseph)
+- [Eric R. Scott](https://github.com/Aariq)
+- [James Tsakalos](https://github.com/jamestsakalos)
+
+<br>
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Angus Watters, Mike J. Johnson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+---
+
+<br>
+
+## How to Contribute
+If you would like to contribute, submit a PR and we will get to as soon as we can!
+If you have any issues please open an issue on GitHub. For any questions, feel free to ask [@anguswg-ucsb](https://github.com/anguswg-ucsb) or [@mikejohnson51](https://github.com/mikejohnson51), or simply create an issue on GitHub.
```

### Comparing `climatePy-0.0.4.1/climatePy/__init__.py` & `climatePy-0.0.4.23/climatePy/__init__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# __init__.py
-import pandas as pd
-import pkg_resources
-
-# warnings lib
-import warnings
-
-# suppress warnings
-warnings.filterwarnings('ignore', category=Warning)
-
-def params():
-    data_file = pkg_resources.resource_filename('climatePy', 'data/catalog.csv')
-    # data_file = pkg_resources.resource_filename('src', 'data/catalog.csv')
-    data = pd.read_csv(data_file, low_memory=False)
-    return data
-
-from ._climatepy_filter import climatepy_filter
-from ._dap import dap, dap_crop, dap_get
-from ._shortcuts import getTerraClim, getTerraClimNormals, getGridMET, getMACA, \
-    get3DEP, getLOCA, getPRISM, getPolaris, \
-    getBCCA, getLivneh, getLivneh_fluxes, getISRIC_soils, getDaymet, \
-    getVIC, getNASADEM, getWorldClim, getCHIRPS, getLCMAP, getNLDAS
-
-# can i do this and get the __all__ to grab all the functions from ._shortcuts.py ?
-# from ._shortcuts import *
-
-__all__ = [
-    'climatepy_filter',
-    'dap',
-    'dap_crop',
-    'dap_get',
-    'getTerraClim',
-    'getTerraClimNormals', 
-    'getGridMET', 
-    'getMACA', 
-    'get3DEP', 
-    'getLOCA', 
-    'getPRISM',
-    'getPolaris', 
-    'getBCCA',
-    'getLivneh', 
-    'getLivneh_fluxes', 
-    'getISRIC_soils', 
-    'getDaymet',
-    'getVIC', 
-    'getNASADEM', 
-    'getWorldClim', 
-    'getCHIRPS', 
-    'getLCMAP',
-    'getNLDAS',
-    'params'
-]
-
-##############################
-# Old method
-# import pandas as pd
-# import pkg_resources
-
-# def params():
-#     data_file = pkg_resources.resource_filename('climatePy', 'data/catalog.csv')
-#     # data_file = pkg_resources.resource_filename('src', 'data/catalog.csv')
-#     data = pd.read_csv(data_file)
-#     return data
-
-# from ._climatepy_filter import *
-# from ._dap import *
-# from ._netrc_utils import *
-# from ._shortcuts import *
+# __init__.py
+import pandas as pd
+import pkg_resources
+
+# warnings lib
+import warnings
+
+# suppress warnings
+warnings.filterwarnings('ignore', category=Warning)
+
+def params():
+    data_file = pkg_resources.resource_filename('climatePy', 'data/catalog.csv')
+    # data_file = pkg_resources.resource_filename('src', 'data/catalog.csv')
+    data = pd.read_csv(data_file, low_memory=False)
+    return data
+
+from ._climatepy_filter import climatepy_filter
+from ._dap import dap, dap_crop, dap_get
+from ._shortcuts import getTerraClim, getTerraClimNormals, getGridMET, getMACA, \
+    get3DEP, getLOCA, getPRISM, getPolaris, \
+    getBCCA, getLivneh, getLivneh_fluxes, getISRIC_soils, getDaymet, \
+    getVIC, getNASADEM, getWorldClim, getCHIRPS, getLCMAP, getNLDAS
+
+# can i do this and get the __all__ to grab all the functions from ._shortcuts.py ?
+# from ._shortcuts import *
+
+__all__ = [
+    'climatepy_filter',
+    'dap',
+    'dap_crop',
+    'dap_get',
+    'getTerraClim',
+    'getTerraClimNormals', 
+    'getGridMET', 
+    'getMACA', 
+    'get3DEP', 
+    'getLOCA', 
+    'getPRISM',
+    'getPolaris', 
+    'getBCCA',
+    'getLivneh', 
+    'getLivneh_fluxes', 
+    'getISRIC_soils', 
+    'getDaymet',
+    'getVIC', 
+    'getNASADEM', 
+    'getWorldClim', 
+    'getCHIRPS', 
+    'getLCMAP',
+    'getNLDAS',
+    'params'
+]
+
+##############################
+# Old method
+# import pandas as pd
+# import pkg_resources
+
+# def params():
+#     data_file = pkg_resources.resource_filename('climatePy', 'data/catalog.csv')
+#     # data_file = pkg_resources.resource_filename('src', 'data/catalog.csv')
+#     data = pd.read_csv(data_file)
+#     return data
+
+# from ._climatepy_filter import *
+# from ._dap import *
+# from ._netrc_utils import *
+# from ._shortcuts import *
 # from ._utils import *
```

### Comparing `climatePy-0.0.4.1/climatePy/_dap.py` & `climatePy-0.0.4.23/climatePy/_dap.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1634 +1,1634 @@
-# date and string parsing libraries
-from datetime import datetime, timedelta, timezone
-from dateutil.parser import parse
-from dateutil import tz
-import re
-
-# spatial data libraries
-import shapely
-from shapely.ops import transform
-from shapely.geometry import mapping
-import geopandas as gpd
-from rtree import index
-import xarray as xr
-import rasterio as rio
-import rioxarray as rxr
-from pyproj import CRS, Proj
-import netCDF4 as nc
-import inspect
-
-# data wrangling and manipulation
-import numpy as np
-import pandas as pd
-
-# library for parallel processing
-from joblib import Parallel, delayed
-
-# import climatePy modules
-from . import _utils as utils
-from . import _climatepy_filter as climatepy_filter
-
-# warnings lib
-import warnings
-
-# suppress warnings
-warnings.filterwarnings('ignore', category=Warning)
-
-# from src.climatePy import climatepy_filter, utils
-# from climatePy import climatepy_filter, utils
-# import utils from src.climatePy
-# from climatePy import _utils, climatepy_filter
-# from climatePy import _utils, climatepy_filter
-# from climatePy import _utils, climatepy_filter
-# import ._utils as utils
-# import ._climatepy_filter as climatepy_filter
-# import _utils as utils
-# import _climatepy_filter as climatepy_filter
-
-def dap_crop(
-    URL       = None,
-    catalog   = None,
-    AOI       = None, 
-    startDate = None, 
-    endDate   = None,
-    varname   = None, 
-    verbose   = False
-    ):
-    """Crop a catalog entry to a specified area of interest and time period.
-    
-    Args:
-        URL (str, optional): The URL of the catalog entry. Defaults to None.
-        catalog (pd.DataFrame, optional): The catalog dataframe. Defaults to None.
-        AOI (geopandas.GeoDataFrame, optional): The area of interest for cropping. Defaults to None.
-        startDate (str, optional): The start date of the time period. Defaults to None.
-        endDate (str, optional): The end date of the time period. Defaults to None.
-        varname (str or list, optional): The variable name(s) to filter the catalog. Defaults to None.
-        verbose (bool, optional): Flag to control verbosity of progress messages. Defaults to Falser.
-        
-	Returns:
-        pd.DataFrame: The cropped catalog entry.
-    """
-    
-    # if a URL is provided, call read_dap_file
-    if URL is not None:
-
-        # stash metadata
-        catvar  = catalog["variable"].values
-        catmod  = catalog["model"].values
-        catens  = catalog["ensemble"].values
-        catsen  = catalog["scenario"].values
-        catcrs  = catalog["crs"].values
-
-        catalog = utils.read_dap_file(
-            URL                  = URL, 
-            varname              = varname,
-            var_spec             = catalog["variable"].values,
-            var_spec_long        = catalog["varname"].values,
-            id                   = "local",
-            varmeta              = verbose, 
-            stopIfNotEqualSpaced = True
-            )
-        
-        # add missing column to catalog
-        catalog["tiled"] = ""
-        catalog["variable"] = catvar
-        catalog["model"]    = catmod
-        catalog["ensemble"] = catens
-        catalog["scenario"] = catsen
-
-        # replace None values in col1 with a string
-        catalog = catalog.fillna({'crs': catcrs[0]})
-
-    # TIME
-    if startDate is None and endDate is None:
-            catalog["T"]    = "[0:1:" + (catalog['nT'] - 1).astype(int).astype(str) + "]"
-            catalog["Tdim"] = catalog["nT"]
-            
-            tmp = [i.split("/") for i in catalog["duration"]]
-            catalog = catalog.assign(startDate = [i[0] for i in tmp], endDate = [i[1] for i in tmp])
-    else:
-        if endDate is None:
-            endDate = startDate
-        
-        # check if its hourly date
-        if any(keyword in catalog['interval'].iloc[0] for keyword in ["hour", "hours"]):
-            startDate += " 00:00:00"
-            endDate   += " 23:00:00"
-
-        # Convert startDate and endDate to pandas Timestamp objects
-        startDate = pd.Timestamp(startDate)
-        endDate   = pd.Timestamp(endDate)
-
-        # out list
-        out = []
-
-        # if interval == "monthly normal" set interval column to "month", otherwise keep interval value
-        catalog.loc[:, "interval"] = np.where(catalog["interval"] == "monthly normal", "month", catalog["interval"])
-        # catalog.loc[:, "interval"] = np.where(catalog["interval"] == "monthly normal", "month", catalog["interval"])
-        
-        # loop over each row of catalog and do date parsing
-        for i in range(len(catalog)): 
-
-            if verbose:
-                print(f'Parsing dates: {i+1}')
-
-            time_steps = parse_date(
-                duration = catalog["duration"].iloc[i], 
-                interval = catalog["interval"].iloc[i]
-                )
-
-            if catalog['nT'].iloc[i] == 1 and not np.isnan(catalog['nT'].iloc[i]):
-                        out.append(pd.concat([
-                                catalog.iloc[[i], :],
-                                pd.DataFrame({
-                                        'T': ['[0:1:0]'],
-                                        'Tdim': [1],
-                                        'startDate': [time_steps[0]],
-                                        'endDate': [time_steps[0]]
-                                })
-                        ], axis=1))
-            elif startDate > max(time_steps) or endDate < min(time_steps):
-                out.append(None)
-                
-            else:
-                T1 = np.argmin(abs(time_steps - startDate))
-                Tn = np.argmin(abs(time_steps - endDate))
-
-                out.append(
-                    pd.concat([catalog.iloc[[i], :].reset_index(drop=True), pd.DataFrame({
-                                                                            'T': [f"[{T1}:1:{Tn}]"],
-                                                                            'Tdim': [(Tn - T1) + 1],
-                                                                            'startDate': [time_steps[T1]],
-                                                                            'endDate': [time_steps[Tn]]
-                                                                            })], axis=1))  
-                                                                
-            # # Concatenate out list of dataframes into single catalog dataframe
-            # catalog = pd.concat(out, axis=0, ignore_index=True)
-
-        # Concatenate out list of dataframes into single catalog dataframe
-        catalog = pd.concat(out, axis=0, ignore_index=True)
-
-        if len(catalog) == 0:
-            raise ValueError(f"Requested Time not found in {set(catalog['duration'])}")
-    
-    # space XY
-    if AOI is None:
-            catalog["X"]    = "[0:1:" + (catalog['ncols'] - 1).astype(int).astype(str) + "]"
-            catalog["Y"]    = "[0:1:" + (catalog['nrows'] - 1).astype(int).astype(str) + "]"
-    else: 
-            # if AOI is given, filter out rows not in AOI bounding box
-            out = []
-
-            # catalog = find_intersects(
-            # 	catalog = catalog,
-            # 	AOI     = AOI
-            # 	)
-
-            # catalog length to track progress
-            n = len(catalog)
-
-            # loop over catalog and filter out rows not in AOI bounding box
-            for i in range(len(catalog)):
-                
-                # print messages if verbose is True
-                if verbose: 
-                    print(f'Filtering out rows not in AOI bounding box: ({i+1}/{n})')
-                
-                # make a bounding box from the catalog row
-                cat_box = utils.make_ext(catalog.iloc[i])
-
-                # make a bounding box from the AOI and reproject to catalog crs
-                aoi_box = AOI.to_crs(catalog["crs"].iloc[0])['geometry'][0].bounds
-
-                # try to intersect the bounding boxes, if it fails append None to out list
-                try:
-                    out.append(shapely.box(*aoi_box).intersection(cat_box))
-                except Exception as e:
-                    out.append(None)
-            # out = Parallel(n_jobs=-1)(delayed(go_get_dap_data) (dap_data.iloc[i].to_dict()) for i in range(len(dap_data)))
-            # find the indices of the None values in out and remove the corresponding rows from catalog
-            drops = [i for i, x in enumerate(out) if x is None]
-        
-            # drop rows from catalog and remove None values from out list
-            if drops:
-                catalog = catalog.drop(drops)
-                out     = [x for x in out if x is not None]
-
-            # catalog length to track progress
-            n = len(catalog)
-
-            # loop over each row and do X/Y coord mapping
-            for i in range(len(catalog)):
-                # print messages if verbose is True
-                if verbose: 
-                    print(f'Mapping X/Y coords: ({i+1}/{n})')
-
-                X_coords = np.linspace(catalog.iloc[i, catalog.columns.get_loc('X1')], catalog.iloc[i, catalog.columns.get_loc('Xn')], num = int(catalog.iloc[i, catalog.columns.get_loc('ncols')]))
-                
-                Y_coords = np.linspace(catalog.iloc[i, catalog.columns.get_loc('Y1')], catalog.iloc[i, catalog.columns.get_loc('Yn')],  num = int(catalog.iloc[i, catalog.columns.get_loc('nrows')]))
-            
-                ys = [np.argmin(np.abs(Y_coords - out[i].bounds[1])), np.argmin(np.abs(Y_coords - out[i].bounds[3]))]
-                xs = [np.argmin(np.abs(X_coords - out[i].bounds[0])), np.argmin(np.abs(X_coords - out[i].bounds[2]))]
-                
-                catalog.loc[i, 'Y'] = f"[{':1:'.join(map(str, sorted(ys)))}]"
-                catalog.loc[i, 'X'] = f"[{':1:'.join(map(str, sorted(xs)))}]"
-
-                catalog.at[i, 'X1'] = min(X_coords[[i + 1 for i in xs]])
-                catalog.at[i, 'Xn'] = max(X_coords[[i + 1 for i in xs]])
-                catalog.at[i, 'Y1'] = min(Y_coords[[i + 1 for i in ys]])
-                catalog.at[i, 'Yn'] = max(Y_coords[[i + 1 for i in ys]])
-                catalog.at[i, 'ncols'] = abs(np.diff(xs))[0] + 1
-                catalog.at[i, 'nrows'] = abs(np.diff(ys))[0] + 1
-    
-    # DIMENSION ORDER STRINGS
-    first  = catalog['dim_order'].str[0].fillna('T').values[0]
-    second = catalog['dim_order'].str[1].fillna('Y').values[0]
-    third  = catalog['dim_order'].str[2].fillna('X').values[0]
-
-    # properly format URL string for tiled data
-    if catalog['tiled'].str.contains('XY').any():
-        catalog['URL'] = catalog['URL'] + '?' + catalog['varname'] + catalog[first] + catalog[second] + catalog[third]
-    else:
-        catalog['URL'] = catalog['URL'] + '?' + catalog['varname'] + catalog[first] + catalog[second] + catalog[third]
-    
-    # check varname
-    if varname is not None:
-        # check if varname is a str, convert to list if so
-        if isinstance(varname, str):
-            varname = [varname]
-        if varname not in catalog['varname'].unique() and varname not in catalog['variable'].unique():
-            var_list = "\t > ".join(catalog['varname'].unique())
-            raise ValueError(f"variable(s) in resource include:\n\t> {var_list}")
-        
-        catalog['varname'] == varname
-        catalog =  catalog.query("varname == @varname")
-
-    # replace NaN values with None
-    catalog = catalog.replace({np.nan: "NA"})
-
-    # TODO: look into what this does, keep commented out for now
-    # catalog["X"] = None
-    # catalog["Y"] = None
-    # catalog["T"] = None
-
-    return catalog
-
-def dap(
-        URL         = None,
-        catalog     = None,
-        AOI         = None,
-        startDate   = None,
-        endDate     = None,
-        varname     = None,
-        grid        = None,
-        start       = None,
-        end         = None,
-        toptobottom = False,
-        dopar       = True,
-        verbose     = False
-        ):
-        
-        """Get data from a DAP server"""
-
-        if not isinstance(toptobottom, bool):
-
-            # print("Checking if all toptobottom values are Nan...")
-
-            # convert to float to check for nan
-            nan_chk = toptobottom.astype(float)
-
-            # if all toptobottom values are Nan, then make toptobottom False 
-            if np.isnan(np.sum(nan_chk)):
-
-                # print("--> setting toptobottom to False")
-                toptobottom = False
-
-        # else:
-        # 	print("toptobottom is already a boolean")
-        # 	print(f"toptobottom = {toptobottom}")
-
-        # check to make sure URL or catalog is provided
-        if URL is None and catalog is None:
-            raise ValueError("URL or catalog must be provided")
-        
-
-        # check if a single string, if so, make a list of string
-        if isinstance(URL, str):
-            URL = [URL]
-
-        # if URL is None then only use catalog URL column
-        if URL is None:
-            URL = catalog.URL.values.tolist()
-
-        else:
-            # convert Numpy array to list
-            url_lst = catalog.URL.values.tolist()
-
-            # extend list with URL
-            url_lst.extend(URL)
-
-            # set URL to list of URLS
-            URL = url_lst
-
-        # check if "vrt" or "tif" in URL list, or if "vsi" in all of URL list
-        if any([utils.getExtension(i) in ['vrt', "tif"] for i in URL]) or all(["vsi" in i for i in URL]):
-
-            if verbose:
-                print("Getting VRT/TIF data")
-                
-            # get the vrt catalog features for each URL
-            vrt_data = vrt_crop_get(
-                URL         = URL,
-                catalog     = catalog,
-                AOI         = AOI,
-                grid        = grid,
-                varname     = varname,
-                start       = start,
-                end         = end,
-                toptobottom = toptobottom,
-                verbose     = False
-                )
-            
-            # # get the vrt catalog features for each URL
-            # vrt_data = vrt_crop_get2(
-            #     URL         = URL,
-            #     catalog     = catalog,
-            #     AOI         = AOI,
-            #     grid        = grid,
-            #     varname     = varname,
-            #     start       = start,
-            #     end         = end,
-            #     toptobottom = toptobottom,
-            #     verbose     = verbose
-            #     )
-            
-            return vrt_data
-
-        else:
-            if verbose:
-                print("Getting DAP data")
-
-            # get the dap catalog features for each URL
-            dap_data = dap_crop(
-                URL       = URL,
-                catalog   = catalog,
-                AOI       = AOI,
-                startDate = startDate,
-                endDate   = endDate,
-                varname   = varname,
-                verbose   = False
-                )
-            
-            # if dopar:
-            #     if verbose:
-            #         print("Getting DAP data in parallel")
-            # else:
-            #     if verbose:
-            #         print("Getting DAP data in serial")
-
-            # get dap data
-            dap_data = dap_get(
-                dap_data = dap_data,
-                dopar    = dopar,
-                verbose  = False
-                )
-            
-            return dap_data
-        
-def match_args(func, *args, **kwargs):
-
-    """Match default arguments for a function.
-
-    This function takes a function and a variable number of positional and keyword arguments.
-    It matches the provided arguments with the default arguments of the function signature
-    and returns a dictionary containing the matched arguments.
-
-    Args:
-        func (callable): The function for which arguments need to be matched.
-        *args: Positional arguments that need to be matched with function parameters.
-        **kwargs: Keyword arguments that need to be matched with function parameters.
-
-    Returns:
-        dict: A dictionary containing the matched arguments as key-value pairs.
-
-    """
-    sig = inspect.signature(func)
-    matched_args = {}
-    for k, v in sig.parameters.items():
-            if k in kwargs:
-                    matched_args[k] = kwargs[k]
-            elif args:
-                    matched_args[k] = args[0]
-                    args = args[1:]
-            else:
-                    matched_args[k] = v.default
-    return matched_args
-
-def climatepy_dap(*args, verbose = False, **kwargs):
-
-        """ClimatePy DAP (DAP).
-        
-        This is an internal function that works to take varied argument inputs and appropriatly match 
-        them to climatepy_filter() and dap_crop() functions. 
-        Args:
-            *args: Positional arguments to be matched with parameters of `climatepy_filter` and `dap_crop`.
-            verbose (bool, optional): Whether to print verbose output during DAP operations. Defaults to False.
-            **kwargs: Keyword arguments to be matched with parameters of `climatepy_filter` and `dap_crop`.
-
-        Returns:
-            dict: A dictionary containing the matched arguments for DAP operations.
-
-        """
-
-        # get matching arguments for climatepy_filter function
-        matches1            = match_args(climatepy_filter.climatepy_filter, *args, **kwargs)
-
-        # get catalog from climatepy_filter
-        x = climatepy_filter.climatepy_filter(**matches1)
-
-        # add catalog to list of arguments that'll be passed to dap
-        matches1['catalog'] = x
-
-        # matches1['verbose'] = True
-        matches1['verbose'] = verbose
-        matches1['varname'] = None
-
-        # match arguments for dap_crop function
-        matches2 = match_args(dap_crop, *args, **kwargs)
-
-        # get matching arguments in climatepy_filter and dap_crop
-        dap_matches = {k: matches1[k] for k in matches1 if k in matches2}
-
-        if verbose: 
-            print("dap_matches: ", dap_matches)
-
-        return dap_matches
-
-def var_to_da(var, dap_row):
-    """Converts a variable to an xarray DataArray with coordinate reference system (CRS).
-
-    Args:
-        var (numpy.ndarray): The variable to be converted to a DataArray.
-        dap_row (pandas.Series): A pandas Series containing metadata information.
-
-    Returns:
-        xarray.DataArray: The variable converted to a DataArray with CRS included.
-
-    """
-
-    # var = get_data(dap_row)
-    # dap_row = dap_row
-
-    # dates = pd.to_datetime(dates)
-    dates = pd.date_range(
-        start   = dap_row['startDate'], 
-        end     = dap_row['endDate'], 
-        periods = dap_row['Tdim']
-        )
-
-    # concatenate variable name with date and model info
-    name = dap_row['variable'] + '_' + dates.strftime('%Y-%m-%d-%H-%M-%S') + '_' + dap_row['model'] + '_' + dap_row['ensemble'] + '_' + dap_row['scenario']
-    name = name.str.replace('_NA', '', regex=False)
-    name = name.str.replace('_na', '', regex=False)
-
-    # extract variable name
-    vars = dap_row['variable']
-
-    # if variable name is NA, use varname
-    if len(vars) == 0:
-        vars = dap_row['varname']
-
-    # clean up timeseries names
-    names_ts = "_".join([vars, dap_row["model"], dap_row["ensemble"], dap_row["scenario"]])
-    names_ts = names_ts.replace("_NA", "")
-    names_ts = names_ts.replace("_na", "")
-    names_ts = names_ts.replace("__", "_")
-    names_ts = names_ts.rstrip("_")
-
-    # if dap_row has 1 column and 1 row, or 1 key/value
-    if len(dap_row.keys()) == 1 and len(dap_row.values()) == 1:
-        # reshape var into a 2D array
-        var_2d = var.reshape((len(dates), -1))
-
-        # create a dictionary of column names and values
-        var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
-        var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
-
-        # create a DataFrame with dates and var_dict as columns
-        df = pd.DataFrame({'date': dates, **var_dict})
-
-    # x resolution
-    resx = (dap_row['Xn'] - dap_row['X1'])/(dap_row['ncols'] - 1)
-
-    # y resolution
-    resy = (dap_row['Yn'] - dap_row['Y1'])/(dap_row['nrows'] - 1)
-
-    xmin = dap_row['X1'] - 0.5 * resx
-    xmax = dap_row['Xn'] + 0.5 * resx
-    ymin = dap_row['Y1'] - 0.5 * resy
-    ymax = dap_row['Yn'] + 0.5 * resy
-
-    # expand dimensions of 'var' if it's a 2D array
-    if var.ndim == 2:
-        var = np.expand_dims(var, axis=-1)
-    
-    # check if size of first dimension of 'var' is equals number of rows in 'dap'
-    if var.shape[2] != dap_row["nrows"]:
-        # transpose the first two dimensions of 'var' if not in correct order
-        var = var.transpose(dap_row["Y_name"], dap_row["X_name"], dap_row["T_name"])
-        # var2 = var.transpose(dap_row["T_name"], dap_row["X_name"],  dap_row["Y_name"])
-    
-    # Create the DataArray with the CRS included
-    r = xr.DataArray(
-        var,
-        coords = {
-            'y': -1*np.linspace(ymin, ymax, dap_row['nrows'], endpoint=False),
-            'x': np.linspace(xmin, xmax, dap_row['ncols'], endpoint=False),
-            'time': dates,
-            'crs': dap_row['crs']
-        },
-        dims=['y', 'x', 'time']
-        )
-
-    # if toptobottom is True, flip the data vertically
-    if dap_row['toptobottom']:
-
-        # vertically flip each 2D array
-        flipped_data = np.flip(r.values, axis=0)
-        # flipped_data = np.flipud(r.values)
-
-        # create new xarray DataArray from flipped NumPy array
-        r = xr.DataArray(
-            flipped_data,
-            dims   = ('y', 'x', 'time'),
-            coords = {'y': r.y, 'x': r.x, 'time': r.time}
-            )
-
-    # set the name attribute of the DataArray
-    r = r.assign_coords(time=name)
-
-    return r
-
-def get_data(dap_row):
-    """Internal function for retrieving data from a DAP (Data Access Protocol) source.
-
-    Args:
-        dap_row (pandas.Series): A pandas Series containing metadata information.
-
-    Returns:
-        xarray.DataArray: The retrieved variable data.
-
-    """
-
-    ds = xr.open_dataset(f"{dap_row['URL']}#fillmismatch")
-
-    var = ds[dap_row['varname']]
-
-    ds.close()
-
-    return var
-
-def go_get_dap_data(dap_row):
-
-    """Internal function for retrieving DAP (Data Access Protocol) data and converting it to a DataArray.
-
-    Args:
-        dap_row (pandas.Series): A pandas Series containing metadata information.
-
-    Returns:
-        xarray.DataArray or str: The retrieved data as a DataArray, or the original URL if an error occurred.
-
-    """
-
-    # dap_row = dap_data.iloc[i].to_dict()
-    try:
-        if "http" in dap_row["URL"]:
-            x = var_to_da(var = get_data(dap_row), dap_row = dap_row)
-        else:
-            raise Exception("dap_to_local() not avaliable, yet, dataset URL must be in http format")
-    except Exception as e:
-        return dap_row["URL"]
-    
-    return x
-
-def add_varname_attr(
-        out = None, 
-        dap_data = None, 
-        verbose = False
-        ):
-    
-    for da, varb in zip(out, dap_data["variable"]):
-        if verbose: 
-            print(f'Adding "variable" attribute {varb} to DataArray')
-        da.attrs["variable"] = varb
-
-    for da, varname in zip(out, dap_data["varname"]):
-        if verbose: 
-            print(f'Adding "var" attribute {varname} to DataArray')
-        da.attrs["varname"] = varname
-
-def merge_across_time(data_arrays, verbose = False):
-
-    """Merge DataArrays across time"""
-
-    if verbose:
-        print("Merging DataArrays across time")
-
-    # create a dictionary to store DataArrays for each unique variable_name
-    da_dict = {}
-
-    n = len(data_arrays)
-
-    for idx, val in enumerate(data_arrays):
-        variable_name = val.attrs.get('variable', 'unknown')
-        # print("Iterating through list of DataArrays: ", variable_name, "-", idx+1, "/", len(data_arrays), " DataArrays")
-
-        if verbose:
-            print(f"Iterating through list of DataArrays: {variable_name} - ({idx+1}/{n})")
-            # print("Iterating through list of DataArrays: ", variable_name)
-
-        if variable_name not in da_dict:
-            if verbose:
-                print("----> variable ", variable_name, "NOT IN da_dict")
-                # print("variable NOT IN da_dict adding dataarray list with key: ", variable_name)
-            da_dict[variable_name] = [val]
-        else:
-            if verbose:
-                print("----> variable ", variable_name, "IN da_dict")
-                # print("variable IN da_dict, appending data array to key: ", variable_name)
-            da_dict[variable_name].append(val)
-
-    # for da in data_arrays:
-    #     variable_name = da.attrs.get('variable_name', 'unknown')
-    #     if variable_name not in da_dict:
-    #         da_dict[variable_name] = [da]
-    #     else:
-    #         da_dict[variable_name].append(da)
-
-    # concatenate DataArrays for each unique variable_name
-    concat_da = []
-    for variable_name, da_list in da_dict.items():
-
-        if verbose:
-            print("--> concatenating time dims: ", variable_name)
-
-        # concatenate DataArrays along the time dimension
-        cda = xr.concat(da_list, dim='time')
-
-        # add variable_name as an attribute to the concatenated DataArray
-        cda.attrs['variable'] = variable_name
-
-        # add the concatenated DataArray to the list of output DataArrays
-        concat_da.append(cda)
-
-    return concat_da
-
-def dap_get(dap_data, dopar = True, varname = None, verbose = False):
-    
-    """Get DAP resource data.
-
-    Args:
-        dap_data (pandas.DataFrame): A DataFrame containing metadata information for DAP resources.
-        dopar (bool, optional): Flag indicating whether to perform parallel execution. Defaults to True.
-        varname (str, optional): The variable name to filter the DAP resources. Defaults to None.
-        verbose (bool, optional): Flag indicating whether to print verbose output. Defaults to False.
-
-    Returns:
-        dict or xarray.DataArray: A dictionary of DataArrays or a single DataArray, representing the retrieved DAP data.
-
-    Raises:
-        ValueError: If the provided varname is not found in the DAP resources.
-
-    """
-    
-    # check if varname is in dap_data
-    if varname is not None:
-        if varname not in dap_data["varname"].values and varname not in dap_data["variable"].values:
-        # if varname not in dap_data['varname'].unique() and varname not in dap_data['variable'].unique():
-            errstr = "\t > ".join(dap_data["varname"].unique())
-            raise ValueError(f'variable(s) in resource include:\n\t > {errstr}' )
-        
-        # filter done dap_data to only include varname if varname is None
-        dap_data = dap_data[
-            (dap_data.get("varname", False) == varname) |
-            (dap_data.get("variable", False) == varname)
-            ]
-        
-    if dopar:
-        # make go_get_dap_data calls in parallel
-        out = Parallel(n_jobs=-1)(delayed(go_get_dap_data) (dap_data.iloc[i].to_dict()) for i in range(len(dap_data)))
-        # out_lst = [go_get_dap_data(dap_row = dap_data.iloc[i].to_dict()) for i in range(len(dap_data))]
-    else:
-        # store output list 
-        out = []
-        # get number of rows in dap_data
-        n = len(dap_data)
-        # # next is to loop over each row in dap_data and call go_get_dap_data
-        for i in range(len(dap_data)):
-            if verbose:
-                print(f'Getting dap data: ({i+1}/{n})')
-
-            x = go_get_dap_data(dap_row = dap_data.iloc[i].to_dict())
-            out.append(x)
-    
-    # add variable name attribute to each DataArray in the output list
-    add_varname_attr(
-        out      = out,
-        dap_data = dap_data, 
-        verbose  = verbose
-        )
-    
-    # merge across time
-    out = merge_across_time(data_arrays = out, verbose = verbose)
-    
-    # concatenated_da = xr.concat(data_arrays, dim=('time', "variable_name"))
-
-    # TODO: USE THIS LIST COMPREHENSION, standard for loop is easier for debugging
-    # next is to loop over each row in dap_data and call go_get_dap_data
-    # out = [go_get_dap_data(dap_data.iloc[x].to_dict()) for x in range(len(dap_data))]
-    # out = [go_get_dap_data(dap_data.iloc[x]) for x in range(len(dap_data))]
-
-    # get data names
-    out_names = list(dict.fromkeys([name.replace("_$", "") for name in dap_data['variable'].tolist()]))
-    # out_names = list(dict.fromkeys([name.replace("_$", "") for name in dap_data['varname'].tolist()]))
-    # out_names = list(set([name.replace("_$", "") for name in dap_data["varname"]]))
-    # out_names = [name.replace("_$", "") for name in dap_data["varname"]]
-    # out_names = dap_data['varname'].str.replace('_$', '').tolist()
-
-    # put list and names into a dictionary
-    out = dict(zip(out_names, out))
-
-    # Check if first DataArray is not a SpatRaster
-    if not isinstance(out[next(iter(out))], xr.core.dataarray.DataArray):
-        if verbose:
-            print("Processing non DataArray data...")
-
-        # out = list(out.values())
-        # out = xr.merge(out, join="outer")
-        # out = reduce(lambda dtf1, dtf2: dtf1.merge(dtf2, on="date", how="outer"), out)
-
-        return out
-    
-    elif any(dap_data["tiled"].str.contains("XY")):
-        if verbose:
-            print("Processing 'XY' data...")
-
-        ll = {}
-        u = np.unique([da.units for da in out])
-
-        if len(u) == 1:
-            out = xr.combine_by_coords(out)
-            out["units"] = (["layer"], [u[0]] * len(out["layer"]))
-            ll[dap["varname"].iloc[0]] = out
-            out = ll
-
-            return out
-        else:
-            # out = dict(zip(out_names, out))
-            return out
-
-    elif any(dap_data["tiled"] == "T"):
-
-        print("Processing 'T' data...")
-
-        # out = xr.concat(out, dim="time").sortby("time")
-        return out
-    else:
-        if verbose:
-            print("Processing as normal...")
-        
-        return out
-
-    return out
-
-def var_to_rast(var, dap_row):
-    """
-    Convert a variable to a raster format.
-
-    Args:
-        var (numpy.ndarray): The variable data to convert.
-        dap_row (pandas.Series): A row from the Data Access Protocol (DAP) climate catalog pandas dataframe containing metadata information.
-
-    Returns:
-        xr.DataArray: The converted variable as a DataArray.
-
-    """
-    
-    # dates = pd.to_datetime(dates)
-    dates = pd.date_range(
-        start   = dap_row['startDate'], 
-        end     = dap_row['endDate'], 
-        periods = dap_row['Tdim']
-        )
-
-    # concatenate variable name with date and model info
-    name = dap_row['variable'] + '_' + dates.strftime('%Y-%m-%d-%H-%M-%S') + '_' + dap_row['model'] + '_' + dap_row['ensemble'] + '_' + dap_row['scenario']
-    name = name.str.replace('_NA', '', regex=False)
-
-    # extract variable name
-    vars = dap_row['variable']
-
-    # if variable name is NA, use varname
-    if len(vars) == 0:
-        vars = dap_row['varname']
-
-    # clean up timeseries names
-    names_ts = "_".join([vars, dap_row["model"], dap_row["ensemble"], dap_row["scenario"]])
-    names_ts = names_ts.replace("_NA", "")
-    names_ts = names_ts.replace("__", "_")
-    names_ts = names_ts.rstrip("_")
-
-    # if dap_row has 1 column and 1 row, or 1 key/value
-    if len(dap_row.keys()) == 1 and len(dap_row.values()) == 1:
-        # reshape var into a 2D array
-        var_2d = var.reshape((len(dates), -1))
-
-        # create a dictionary of column names and values
-        var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
-        var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
-
-        # create a DataFrame with dates and var_dict as columns
-        df = pd.DataFrame({'date': dates, **var_dict})
-
-    # x resolution
-    resx = (dap_row['Xn'] - dap_row['X1'])/(dap_row['ncols'] - 1)
-
-    # y resolution
-    resy = (dap_row['Yn'] - dap_row['Y1'])/(dap_row['nrows'] - 1)
-
-    xmin = dap_row['X1'] - 0.5 * resx
-    xmax = dap_row['Xn'] + 0.5 * resx
-    ymin = dap_row['Y1'] - 0.5 * resy
-    ymax = dap_row['Yn'] + 0.5 * resy
-
-    # expand dimensions of 'var' if it's a 2D array
-    if var.ndim == 2:
-        var = np.expand_dims(var, axis=-1)
-
-    # check if size of first dimension of 'var' is equals number of rows in 'dap'
-    if var.shape[2] != dap_row["nrows"]:
-        # transpose the first two dimensions of 'var' if not in correct order
-        var = var.transpose(dap_row["Y_name"], dap_row["X_name"], dap_row["T_name"])
-        # var2 = var.transpose(dap_row["T_name"], dap_row["X_name"],  dap_row["Y_name"])
-
-    # Create the DataArray with the CRS included
-    r = xr.DataArray(
-        var,
-        coords = {
-            'y': -1*np.linspace(ymin, ymax, dap_row['nrows'], endpoint=False),
-            'x': np.linspace(xmin, xmax, dap_row['ncols'], endpoint=False),
-            'time': dates,
-            'crs': dap_row['crs']
-        },
-        dims=['y', 'x', 'time']
-        )
-
-    # if toptobottom is True, flip the data vertically
-    if dap_row['toptobottom']:
-
-        # vertically flip each 2D array
-        flipped_data = np.flip(r.values, axis=1)
-
-        # create new xarray DataArray from flipped NumPy array
-        r = xr.DataArray(
-            flipped_data,
-            dims   = ('y', 'x', 'time'),
-            coords = {'y': r.y, 'x': r.x, 'time': r.time}
-            )
-        
-    # set the name attribute of the DataArray
-    r = r.assign_coords(time=name)
-
-    return r
-
-def do_dap(catalog, AOI, varname, verbose = False):
-        dap_data = dap(
-            catalog = catalog,
-            AOI     = AOI,
-            verbose = verbose
-            )
-        return dap_data[varname]
-
-def repeat_durations(start_date, end_date, repeat_count):
-    """Repeat durations between start_date and end_date.
-
-    Args:
-        start_date (str or datetime): Start date of the duration.
-        end_date (str or datetime): End date of the duration.
-        repeat_count (int): Number of times to repeat the durations.
-
-    Returns:
-        list: List of repeated durations in the format 'YYYY-MM-DD/YYYY-MM-DD'.
-    """
-    date_list = pd.date_range(start=start_date, end=end_date, freq='D').tolist()
-    repeated_dates = []
-    for date in date_list:
-        for i in range(repeat_count):
-            repeated_dates.append(date)
-    durs = [f'{i.strftime("%Y-%m-%d")}/{i.strftime("%Y-%m-%d")}' for i in repeated_dates]
-    return durs
-
-def get_prism_daily(AOI, varname, startDate, endDate, verbose = False):
-
-    """Retrieve PRISM daily climate data.
-
-    Args:
-        AOI (str): Area of interest.
-        varname (str): Variable name.
-        startDate (str or datetime): Start date of the data.
-        endDate (str or datetime): End date of the data.
-        verbose (bool): Verbosity flag.
-
-    Returns:
-        dict: Dictionary containing the retrieved climate data.
-    """
-        
-    # collect raw meta data
-    raw = climatepy_filter.climatepy_filter(
-        id        = "prism_daily", 
-        AOI       = AOI, 
-        varname   = varname,
-        startDate = startDate,
-        endDate   = endDate
-    )
-
-    if endDate is None:
-        endDate = startDate
-
-    # collect varname in correct order
-    varname = raw.varname.unique().tolist()
-
-    # for i in range(len(varname)):
-    #     # make dates for each variable
-    #     pd.date_range(start=startDate, end=endDate, freq='D').tolist()
-    # convert to datetime objects and create date range
-    dates = pd.date_range(start=startDate, end=endDate, freq='D').tolist()
-
-    # create new DataFrame with xx column for each date in dates
-    out = [raw.assign(x=date) for date in dates]
-    
-    # concatenate all DataFrames into a single DataFrame
-    out = pd.concat(out, ignore_index=True)
-
-    # add YYYY column
-    out = out.assign(YYYY=out['x'].apply(lambda x: x.year))
-
-    # convert datetime column to YYYY-MM-DD string format
-    out['x'] = out['x'].dt.strftime('%Y-%m-%d')
-
-    # create a YYYYMMDD column from string date
-    out = out.assign(YYYYMMDD=out['x'].apply(lambda x: x.replace("-", "")))
-
-    # define lambda function to replace substrings in URL column
-    replace_values = lambda x: x['URL'].replace('{YYYY}', str(x['YYYY'])).replace('{YYYYMMDD}', str(x['YYYYMMDD']))
-
-    # apply lambda function to DataFrame
-    out['URL'] = out.apply(replace_values, axis=1)
-
-    # add duration column
-    out['duration'] = repeat_durations(startDate, endDate, len(varname))
-    # out['duration'] = [f'{i.strftime("%Y-%m-%d")}/{i.strftime("%Y-%m-%d")}' for i in dates]
-
-    # from joblib import Parallel, delayed, parallel_backend
-    out_lst = Parallel(n_jobs=-1)(delayed(do_dap) (catalog = out.iloc[[i]], 
-                                                AOI  = AOI,
-                                                varname = out.varname.iloc[i], 
-                                                verbose = False
-                                                ) for i in range(len(out)))
-    # out_lst = []
-    # for i in range(len(out)):
-        
-    #     dap_data = do_dap(
-    #         catalog = out.iloc[[i]],
-    #         AOI     = AOI,
-    #         varname = out.varname.iloc[i],
-    #         verbose = verbose
-    #     )
-        # out_lst.append(dap_data)
-        # out_lst.append(dap_data[out.varname.iloc[i]])
-    
-    out_lst = merge_across_time(out_lst)
-
-    # type(out_lst[0])
-    # get data names
-    out_names = list(dict.fromkeys([name.replace("_$", "") for name in out['variable'].tolist()]))
-
-    # put list and names into a dictionary
-    out = dict(zip(out_names, out_lst))
-
-    return out
-
-def get_nodata(dtype):
-    """Returns the NoData value based on the data type.
-
-    Args:
-        dtype (str): The data type string.
-
-    Returns:
-        The NoData value corresponding to the data type. If the data type is 'int', returns 0. If the data type is 'float',
-        returns np.nan. If the data type is 'uint', returns 0. If the data type is 'complex', returns 0 + 0j. If the data
-        type is 'bool', returns False. For any other data type, returns None.
-    """
-
-    if "int" in dtype:
-        return 0
-    elif "float" in dtype:
-        # return 0.0 if dtype == "float32" or dtype == "float64" else np.nan
-        return np.nan
-    elif "uint" in dtype:
-        return 0
-    elif "complex" in dtype:
-        return 0 + 0j
-    elif "bool" in dtype:
-        return False
-    else:
-        return None
-    
-
-def crop_vrt2(urls, AOI, verbose = False):
-
-    """Crop a VRT to an AOI"""
-
-    # Function for opening a single VRT file with rasterio
-    def crop_vrt_for_url(url, AOI, verbose):
-        
-        with rio.open(url) as src:
-            if verbose: 
-                print('Source tags:', src.tags(1))
-                print("Source desc: ", src.descriptions)
-                print("Source profile: ", src.profile)
-
-            # Reproject the geometry to the CRS of the DataArray
-            AOIv = AOI.to_crs(src.crs, inplace=False)
-
-            # Get the bounding box of your AOI shape
-            bbox = AOIv.geometry.total_bounds
-
-            # Create a polygon object representing the bounding box
-            bounding_box = shapely.geometry.box(bbox[0], bbox[1], bbox[2], bbox[3])
-
-            if verbose:
-                print(" Cropping VRT to bounding box...")
-
-            # check data types and get nodata value
-            dtype   = src.profile['dtype']
-            no_data = get_nodata(dtype)
-
-            print("dtype: ", dtype)
-            print("nodata: ", no_data)
-
-            # out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, invert = False)
-            out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, nodata = no_data, invert = False)
-            out_meta = src.meta
-            out_tags = src.tags(1)
-
-            # if nodata in out_meta, replace nodata value with value used as nodata
-            if 'nodata' in out_meta:
-                out_meta['nodata'] = no_data
-
-            # if nodata in out_tags, replace nodata value with value used as nodata
-            if 'nodata' in out_tags:
-                out_tags['nodata'] = no_data
-
-            # out_image, out_transform = rio.mask.mask(src, AOIv.geometry, crop=True, nodata=np.nan, invert = False)
-            # out_meta = src.meta
-            
-            # close the dataset
-            src.close()
-
-        if out_image.ndim == 3:
-            out_image = out_image.squeeze()
-
-        # bb = AOI.geometry.total_bounds
-        # rio.windows.from_bounds(*bb, out_transform)
-
-        # get height and width of image
-        height = out_image.shape[0]
-        width = out_image.shape[1]
-
-        # get x and y width height indices
-        x_indices = np.arange(width)
-        y_indices = np.arange(height)
-
-        # create meshgrid
-        x_coords, y_coords = np.meshgrid(x_indices, y_indices)
-
-        # get affine transform for coordinates
-        x_coords, y_coords = rio.transform.xy(out_transform, y_coords, x_coords)
-
-        # stack the arrays along a new dimension
-        coords = np.stack((x_coords, y_coords), axis=-1)
-
-        # x and y stacks
-        xn = np.stack((x_coords), axis=-1)
-        yn = np.stack((y_coords), axis=-1)
-
-        # get min and max of x and y
-        xmin = xn.min()
-        xmax = xn.max()
-        ymin = yn.min()
-        ymax = yn.max()
-
-        # # GET CRS
-        # crs = out_meta['crs']
-
-        # create DataArray
-        r = xr.DataArray(
-            out_image,
-            coords={
-                'y': -1*np.linspace(ymin, ymax, height, endpoint=False),
-                'x': np.linspace(xmin, xmax, width, endpoint=False),
-            },
-            dims=['y', 'x']
-        )
-
-        # add tags to attributes of data array
-        for key, value in out_tags.items():
-            r.attrs[key] = value
-
-        # add tags to attributes of data array
-        for key, value in out_meta.items():
-            r.attrs[key] = value
-
-        return r
-    
-
-    # tmp = crop_vrt_for_url(urls[1], AOI, verbose = True)
-    results = Parallel(n_jobs=-1)(delayed(crop_vrt_for_url) (url = i,
-                                            AOI  = AOI,
-                                            verbose = False
-                                            ) for i in urls)
-    
-    return results
-
-def crop_vrt(urls, AOI, verbose = False):
-
-    """Crop a VRT to an AOI"""
-
-    # make empty list to store dataarrays
-    da_lst = []
-
-    # loop over each url
-    for url in urls:
-        with rio.open(url) as src:
-            if verbose: 
-                print('Source tags:', src.tags(1))
-                print("Source desc: ", src.descriptions)
-                print("Source profile: ", src.profile)
-
-            # Reproject the geometry to the CRS of the DataArray
-            AOIv = AOI.to_crs(src.crs, inplace=False)
-
-            # Get the bounding box of your AOI shape
-            bbox = AOIv.geometry.total_bounds
-
-            # Create a polygon object representing the bounding box
-            bounding_box = shapely.geometry.box(bbox[0], bbox[1], bbox[2], bbox[3])
-
-            if verbose:
-                print(" Cropping VRT to bounding box...")
-
-            # check data types and get nodata value
-            dtype   = src.profile['dtype']
-            no_data = get_nodata(dtype)
-
-            print("dtype: ", dtype)
-            print("nodata: ", no_data)
-
-            # out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, invert = False)
-            out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, nodata = no_data, invert = False)
-            out_meta = src.meta
-            out_tags = src.tags(1)
-
-            # if nodata in out_meta, replace nodata value with value used as nodata
-            if 'nodata' in out_meta:
-                out_meta['nodata'] = no_data
-
-            # if nodata in out_tags, replace nodata value with value used as nodata
-            if 'nodata' in out_tags:
-                out_tags['nodata'] = no_data
-
-            # out_image, out_transform = rio.mask.mask(src, AOIv.geometry, crop=True, nodata=np.nan, invert = False)
-            # out_meta = src.meta
-            
-            # close the dataset
-            src.close()
-
-        if out_image.ndim == 3:
-            out_image = out_image.squeeze()
-
-        # bb = AOI.geometry.total_bounds
-        # rio.windows.from_bounds(*bb, out_transform)
-
-        # get height and width of image
-        height = out_image.shape[0]
-        width = out_image.shape[1]
-
-        # get x and y width height indices
-        x_indices = np.arange(width)
-        y_indices = np.arange(height)
-
-        # create meshgrid
-        x_coords, y_coords = np.meshgrid(x_indices, y_indices)
-
-        # get affine transform for coordinates
-        x_coords, y_coords = rio.transform.xy(out_transform, y_coords, x_coords)
-
-        # stack the arrays along a new dimension
-        coords = np.stack((x_coords, y_coords), axis=-1)
-
-        # x and y stacks
-        xn = np.stack((x_coords), axis=-1)
-        yn = np.stack((y_coords), axis=-1)
-
-        # get min and max of x and y
-        xmin = xn.min()
-        xmax = xn.max()
-        ymin = yn.min()
-        ymax = yn.max()
-
-        # # GET CRS
-        # crs = out_meta['crs']
-
-        # create DataArray
-        r = xr.DataArray(
-            out_image,
-            coords={
-                'y': -1*np.linspace(ymin, ymax, height, endpoint=False),
-                'x': np.linspace(xmin, xmax, width, endpoint=False),
-            },
-            dims=['y', 'x']
-        )
-
-        # add tags to attributes of data array
-        for key, value in out_tags.items():
-            r.attrs[key] = value
-
-        # add tags to attributes of data array
-        for key, value in out_meta.items():
-            r.attrs[key] = value
-        # [r.attrs.update({key: value}) for key, value in out_tags.items()]    
-
-        da_lst.append(r)
-        # dataarrays[url] = r
-
-    return da_lst
-
-def vrt_crop_get(
-        URL         = None, 
-        catalog     = None, 
-        AOI         = None, 
-        grid        = None,
-        varname     = None, 
-        start       = None, 
-        end         = None, 
-        toptobottom = False, 
-        verbose     = False
-        ):
-    
-#     """
-#     Crop and process VRT data.
-
-#     Args:
-#         URL (str or list, optional): The URL(s) of the VRT file(s) to open. If not provided, it is extracted from the catalog.
-#         catalog (object, optional): The catalog object containing the URL(s) of the VRT file(s). Required if URL is not provided.
-#         AOI (geopandas.GeoDataFrame, optional): The Area of Interest polygon to crop the VRT data to.
-#         grid (object, optional): The grid object defining the extent and CRS for cropping and reprojection.
-#         varname (str, optional): The name of the variable to select from the VRT data.
-#         start (int, optional): The start index for subsetting bands in the VRT data.
-#         end (int, optional): The end index for subsetting bands in the VRT data.
-#         toptobottom (bool, optional): Whether to flip the data vertically.
-#         verbose (bool, optional): Whether to print informative messages during processing. Default is False
-
-#     Returns:
-#         xr.DataArray: The cropped and processed VRT data.
-
-#     """
-
-    if URL is None:
-        URL = catalog.URL.to_list()
-
-    if verbose:
-        print("Opening VRT from URL: ", URL)
- 
-    # Area of interest
-    vrts = crop_vrt(urls = URL, AOI = AOI, verbose = verbose)
-
-    # vrts2 = Parallel(n_jobs=-1)(delayed(crop_vrt) (urls = [i],
-    #                                     AOI  = AOI,
-    #                                     verbose = False
-    #                                     ) for i in URL)
-
-    # check if data needs to be vertically flipped
-    for idx, val in enumerate(catalog['toptobottom']):
-
-        if verbose:
-            print("idx:", idx, "val: ",val)
-
-        if val and not np.isnan(val):
-
-            if verbose:
-                print("Flipping data vertically")
-            # vertically flip each 2D array
-            flipped_data = np.flip(vrts[idx].values, axis=0)
-
-            # stash tags
-            tags = vrts[idx].attrs
-
-            # create new xarray DataArray from flipped NumPy array
-            vrts[idx] = xr.DataArray(
-                flipped_data,
-                dims   = ('y', 'x'),
-                coords = {'y': vrts[idx].y, 'x': vrts[idx].x}
-                )
-            
-            # add tags back to flipped DataArray
-            vrts[idx].attrs = tags
-
-        else:
-            if verbose:
-                print("Not flipping data vertically")
-            # vrts[idx] = np.flip(vrts[idx], axis=0)
-
-    # create dictionary of DataArrays
-    vrts = dict(zip(catalog['variable'], vrts))
-
-    return vrts
-
-def parse_date(duration, interval):
-        """Parse the date range based on the duration and interval.
-
-        Args:
-            duration (str): The duration string in the format "start_date/end_date".
-            interval (str): The interval string specifying the time unit.
-        
-        Returns:
-            pd.DatetimeIndex: A pandas DatetimeIndex representing the parsed date range.
-        """
-        
-        # split duration string
-        d = duration.split("/")
-        
-        # if end date is "..", set it to today's date
-        if d[1] == "..":
-                d[1] = datetime.now().strftime("%Y-%m-%d")
-
-        # if interval in ["1 month", "1 months"]:
-        if any(keyword in interval for keyword in ["1 month", "1 months", "monthly"]):
-        # if any(keyword in interval for keyword in ["1 month", "1 months", "31 days", "monthly"]):
-                d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-01")
-
-        # if interval in ["hour", "hours"]:
-        if any(keyword in interval for keyword in ["hour", "hours"]):
-                d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
-                d[1] = datetime.strptime(d[1], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
-
-        # if interval is 31 days, change to 1 month
-        if interval in ["31 days","31.5 days"]:
-            interval = "1 month"
-
-        # if interval is 365, 365.5 days, change to 1 year
-        if interval in ["365 days","365.5 days"]:
-            interval = "1 year"
-
-        interval_map = {
-            "hour": "H",
-            "hours": "H",
-            "minute": "min",
-            "minutes": "min",
-            "second": "S",
-            "seconds": "S",
-            "month": "MS",  # Month Start
-            "months": "MS"  # Month Start
-            }
-        
-        # split interval string
-        interval_type = interval.split(" ")[-1]
-
-        # get frequency from interval_map
-        freq = interval_map.get(interval_type, interval_type[0])
-        
-        # # convert start_date and end_date to pandas Timestamp objects
-        # start_date = pd.Timestamp(d[0])
-        # end_date = pd.Timestamp(d[1])
-        # # calculate the number of days between start and end dates
-        # delta = (end_date - start_date) / (nT - 1)
-        # # generate the date range
-        # date_range = pd.date_range(start=start_date, end=end_date, freq=str(int(delta.days))+'D')
-
-        return pd.date_range(start=d[0], end=d[1], freq=freq)
-
-# def parse_date2(duration, nT):
-    # duration = catalog["duration"].iloc[i]
-    # interval = catalog["interval"].iloc[i]
-    # nT = catalog["nT"].iloc[i]
-#     d = duration.split("/")
-#     if d[1] == "..":
-#         d[1] = pd.Timestamp.today().strftime("%Y-%m-%d")
-#     duration = pd.to_datetime(d[1]) - pd.to_datetime(d[0])
-#     start_date = pd.to_datetime(d[0])
-#     end_date = pd.to_datetime(d[1])
-#     duration_in_days = (end_date - start_date).days
-
-#     # calculate interval in days
-#     interval_in_days = duration_in_days / nT
-# 	interval_in_days = 31
-#     # calculate the number of days to shift the frequency
-#     days_to_shift = (start_date + pd.offsets.MonthBegin(1) - start_date).days
-    
-#     # create frequency string with the offset of days to shift
-#     freq = str(int(interval_in_days)) + 'D'
-#     freq = pd.tseries.offsets.DateOffset(days=days_to_shift) 
-#     # + pd.tseries.offsets.CustomBusinessDay(n=interval_in_days)
-#     return pd.date_range(start=start_date, end=end_date, freq=freq)
-# 	interval_in_days = duration / nT
-#     if interval_in_days >= pd.Timedelta(days=365):
-#         freq = 'AS'
-#     elif interval_in_days >= pd.Timedelta(days=30):
-#         freq = 'M'
-#     elif interval_in_days >= pd.Timedelta(days=1):
-#         freq = 'D'
-#     else:
-#         freq = 'H'
-#     return pd.date_range(start=d[0], end=d[1], freq=freq)
-
-# def parse_date2(duration, interval):
-#     d = duration.split("/")
-#     if d[1] == "..":
-#         d[1] = datetime.now().strftime("%Y-%m-%d")
-#     # Get the start and end dates
-#     start_date, end_date = map(lambda x: datetime.strptime(x, '%Y-%m-%d'), d)
-
-#     # Set the start date to the first day of the month
-#     start_date = start_date.replace(day=1)
-#     if "hour" in interval:
-#         # Truncate the start and end dates to the nearest hour
-#         start_date = start_date.replace(minute=0, second=0)
-#         end_date = end_date.replace(minute=0, second=0)
-#     # interval_map = {
-#     #     "hour": "%H",
-#     #     "hours": "%H",
-#     #     "minute": "%M",
-#     #     "minutes": "%M",
-#     #     "second": "%S",
-#     #     "seconds": "%S",
-#     #     "month": "MS",  # Month Start
-# 	# 	"months": "MS"  # Month Start
-#     # }
-#     interval_type = interval.split(" ")[-1]
-#     print("interval_type: ", interval_type)
-#     freq = interval_map.get(interval_type, interval_type[0])
-#     print("frequency date: ", freq)
-#     return pd.date_range(start=d[0], end=d[1], freq=freq)
-#     # return pd.date_range(start=start_date.strftime("%Y-%m-%d"), end=end_date.strftime("%Y-%m-%d"), freq=freq)
-# def filter_row(i, catalog, AOI):
-#     # make a bounding box from the catalog row
-#     cat_box = make_ext(catalog.iloc[i])
-#     # make a bounding box from the AOI and reproject to catalog crs
-#     aoi_box = AOI.to_crs(catalog["crs"].iloc[0])['geometry'][0].bounds
-#     # try to intersect the bounding boxes, if it fails append None to out list
-#     try:
-#         return shapely.box(*aoi_box).intersection(cat_box)
-#     except Exception as e:
-#         return None
-
-# def vrt_crop_get2(
-#         URL         = None, 
-#         catalog     = None, 
-#         AOI         = None, 
-#         grid        = None,
-#         varname     = None, 
-#         start       = None, 
-#         end         = None, 
-#         toptobottom = False, 
-#         verbose     = False
-#         ):
-    
-#     """
-#     Crop and process VRT data.
-
-#     Args:
-#         URL (str or list, optional): The URL(s) of the VRT file(s) to open. If not provided, it is extracted from the catalog.
-#         catalog (object, optional): The catalog object containing the URL(s) of the VRT file(s). Required if URL is not provided.
-#         AOI (geopandas.GeoDataFrame, optional): The Area of Interest polygon to crop the VRT data to.
-#         grid (object, optional): The grid object defining the extent and CRS for cropping and reprojection.
-#         varname (str, optional): The name of the variable to select from the VRT data.
-#         start (int, optional): The start index for subsetting bands in the VRT data.
-#         end (int, optional): The end index for subsetting bands in the VRT data.
-#         toptobottom (bool, optional): Whether to flip the data vertically.
-#         verbose (bool, optional): Whether to print informative messages during processing.
-
-#     Returns:
-#         xr.DataArray: The cropped and processed VRT data.
-
-#     """
-
-#     if URL is None:
-#         URL = catalog.URL.to_list()
-
-#     if verbose:
-#         print("Opening VRT from URL: ", URL)
-
-#     # Read in each file as a separate DataArray and put them in a list
-#     vrts = [xr.open_rasterio(url) for url in URL]
-
-#     # Concatenate the DataArrays along the band dimension
-
-#     if len(vrts) == 1:
-#         vrts = vrts[0]
-#     else:
-#         vrts = xr.concat(vrts, dim="band")
-    
-#     # open VRT
-#     # with xr.set_options(keep_attrs=True):
-#     # vrts = rxr.open_rasterio(URL[0])
-
-#     # index number and name of index for subsetting bands
-#     # var_idx = vrts.attrs['long_name'].index(varname.item()) 
-#     # var_key = [i for i in vrts.attrs['long_name'] if i == varname.item()]
-
-#     # if varname is Not none
-#     if varname is not None:
-        
-#         # vrts = vrts.isel(band=vrts.attrs['long_name'].index(varname.item()))
-#         if "long_name" in vrts.attrs.keys():
-
-#             if verbose:
-#                 print("Selecting varnames")
-#             vrts = vrts.sel(band = vrts.attrs['long_name'].index(varname.tolist()[0]))
-
-#     # subset by index if non "date" dimension
-#     if start is not None and end is None:
-#         vrts = vrts.isel(band=start)
-#     elif start is not None and end is not None:
-#         vrts = vrts.isel(band=slice(start, end))
-
-#     if grid is not None:
-#         xmin = grid.extent[0]
-#         ymin = grid.extent[1]
-#         xmax = grid.extent[2]
-#         ymax = grid.extent[3]
-
-#         # clip vrts to grid extent
-#         vrts = vrts.rio.clip_box(xmin, ymin, xmax, ymax)
-        
-#         # reproject vrts to grid CRS
-#         vrts.rio.write_crs(grid.crs, inplace=True)
-
-#         # flag as True if grid is given
-#         flag = True
-#     else:
-#         if (vrts.rio.crs.to_string() is None or vrts.rio.crs.to_string() == "") or all([i in [0, 1, 0, 1] for i in vrts.rio.bounds()]):
-#             if verbose:
-#                 print("Defined URL(s) are aspatial and on a unit grid. Cannot be cropped")
-
-#             # flag as False if missing CRS or if bounding box is [0, 1, 0, 1]
-#             flag = False
-#         else:
-#             # flag as True if no grid is given and nothing noteworthy
-#             flag = True
-
-#     # if an AOI is given and no flagging happens, crop and mask rasters to AOI
-#     if AOI is not None and flag:
-
-#         # Reproject the geometry to the CRS of the DataArray
-#         AOIv = AOI.to_crs(vrts.rio.crs)
-    
-#         # reproject AOI to vrts CRS
-#         # AOIv = AOI.to_crs(vrts.rio.crs, inplace=False).geometry.apply(lambda x: (x, 1))
-
-#         if verbose:
-#             print("Cropping/Clipping to AOI")
-#         # vrts.rio.
-#         # Crop the raster to the extent of the AOI
-#         # Crop and mask the DataArray to the polygon
-#         vrts = vrts.rio.clip(AOIv.geometry.apply(mapping))
-
-#         # dim that is NOT x or y
-#         selected_dim = [dim for dim in vrts.dims if dim not in ['x', 'y']][0]
-
-#         if "long_name" in vrts.attrs.keys():
-#             # delete extra long_name attributes
-#             del vrts.attrs['long_name']
-    
-#     # if toptobottom is True, flip the data vertically
-#     if toptobottom:
-        
-#         # print("Flipping data toptobottom")
-#         if verbose:
-#             print("Flipping data vertically")
-
-#         # vertically flip each 2D array
-#         flipped_data = np.flip(vrts.values, axis=0)
-
-#         # create new xarray DataArray from flipped NumPy array
-#         vrts = xr.DataArray(
-#             flipped_data,
-#             dims   = ('band', 'y', 'x'),
-#             coords = {'band': vrts[selected_dim], 'y': vrts.y, 'x': vrts.x}
-#             # dims   = ('y', 'x', 'time'),
-#             # coords = {'y': vrts_crop.y, 'x': vrts_crop.x, 'time': vrts_crop.time}
-#             )
-#     # vrts.close()
-
+# date and string parsing libraries
+from datetime import datetime, timedelta, timezone
+from dateutil.parser import parse
+from dateutil import tz
+import re
+
+# spatial data libraries
+import shapely
+from shapely.ops import transform
+from shapely.geometry import mapping
+import geopandas as gpd
+from rtree import index
+import xarray as xr
+import rasterio as rio
+import rioxarray as rxr
+from pyproj import CRS, Proj
+import netCDF4 as nc
+import inspect
+
+# data wrangling and manipulation
+import numpy as np
+import pandas as pd
+
+# library for parallel processing
+from joblib import Parallel, delayed
+
+# import climatePy modules
+from . import _utils as utils
+from . import _climatepy_filter as climatepy_filter
+
+# warnings lib
+import warnings
+
+# suppress warnings
+warnings.filterwarnings('ignore', category=Warning)
+
+# from src.climatePy import climatepy_filter, utils
+# from climatePy import climatepy_filter, utils
+# import utils from src.climatePy
+# from climatePy import _utils, climatepy_filter
+# from climatePy import _utils, climatepy_filter
+# from climatePy import _utils, climatepy_filter
+# import ._utils as utils
+# import ._climatepy_filter as climatepy_filter
+# import _utils as utils
+# import _climatepy_filter as climatepy_filter
+
+def dap_crop(
+    URL       = None,
+    catalog   = None,
+    AOI       = None, 
+    startDate = None, 
+    endDate   = None,
+    varname   = None, 
+    verbose   = False
+    ):
+    """Crop a catalog entry to a specified area of interest and time period.
+    
+    Args:
+        URL (str, optional): The URL of the catalog entry. Defaults to None.
+        catalog (pd.DataFrame, optional): The catalog dataframe. Defaults to None.
+        AOI (geopandas.GeoDataFrame, optional): The area of interest for cropping. Defaults to None.
+        startDate (str, optional): The start date of the time period. Defaults to None.
+        endDate (str, optional): The end date of the time period. Defaults to None.
+        varname (str or list, optional): The variable name(s) to filter the catalog. Defaults to None.
+        verbose (bool, optional): Flag to control verbosity of progress messages. Defaults to Falser.
+        
+	Returns:
+        pd.DataFrame: The cropped catalog entry.
+    """
+    
+    # if a URL is provided, call read_dap_file
+    if URL is not None:
+
+        # stash metadata
+        catvar  = catalog["variable"].values
+        catmod  = catalog["model"].values
+        catens  = catalog["ensemble"].values
+        catsen  = catalog["scenario"].values
+        catcrs  = catalog["crs"].values
+
+        catalog = utils.read_dap_file(
+            URL                  = URL, 
+            varname              = varname,
+            var_spec             = catalog["variable"].values,
+            var_spec_long        = catalog["varname"].values,
+            id                   = "local",
+            varmeta              = verbose, 
+            stopIfNotEqualSpaced = True
+            )
+        
+        # add missing column to catalog
+        catalog["tiled"] = ""
+        catalog["variable"] = catvar
+        catalog["model"]    = catmod
+        catalog["ensemble"] = catens
+        catalog["scenario"] = catsen
+
+        # replace None values in col1 with a string
+        catalog = catalog.fillna({'crs': catcrs[0]})
+
+    # TIME
+    if startDate is None and endDate is None:
+            catalog["T"]    = "[0:1:" + (catalog['nT'] - 1).astype(int).astype(str) + "]"
+            catalog["Tdim"] = catalog["nT"]
+            
+            tmp = [i.split("/") for i in catalog["duration"]]
+            catalog = catalog.assign(startDate = [i[0] for i in tmp], endDate = [i[1] for i in tmp])
+    else:
+        if endDate is None:
+            endDate = startDate
+        
+        # check if its hourly date
+        if any(keyword in catalog['interval'].iloc[0] for keyword in ["hour", "hours"]):
+            startDate += " 00:00:00"
+            endDate   += " 23:00:00"
+
+        # Convert startDate and endDate to pandas Timestamp objects
+        startDate = pd.Timestamp(startDate)
+        endDate   = pd.Timestamp(endDate)
+
+        # out list
+        out = []
+
+        # if interval == "monthly normal" set interval column to "month", otherwise keep interval value
+        catalog.loc[:, "interval"] = np.where(catalog["interval"] == "monthly normal", "month", catalog["interval"])
+        # catalog.loc[:, "interval"] = np.where(catalog["interval"] == "monthly normal", "month", catalog["interval"])
+        
+        # loop over each row of catalog and do date parsing
+        for i in range(len(catalog)): 
+
+            if verbose:
+                print(f'Parsing dates: {i+1}')
+
+            time_steps = parse_date(
+                duration = catalog["duration"].iloc[i], 
+                interval = catalog["interval"].iloc[i]
+                )
+
+            if catalog['nT'].iloc[i] == 1 and not np.isnan(catalog['nT'].iloc[i]):
+                        out.append(pd.concat([
+                                catalog.iloc[[i], :],
+                                pd.DataFrame({
+                                        'T': ['[0:1:0]'],
+                                        'Tdim': [1],
+                                        'startDate': [time_steps[0]],
+                                        'endDate': [time_steps[0]]
+                                })
+                        ], axis=1))
+            elif startDate > max(time_steps) or endDate < min(time_steps):
+                out.append(None)
+                
+            else:
+                T1 = np.argmin(abs(time_steps - startDate))
+                Tn = np.argmin(abs(time_steps - endDate))
+
+                out.append(
+                    pd.concat([catalog.iloc[[i], :].reset_index(drop=True), pd.DataFrame({
+                                                                            'T': [f"[{T1}:1:{Tn}]"],
+                                                                            'Tdim': [(Tn - T1) + 1],
+                                                                            'startDate': [time_steps[T1]],
+                                                                            'endDate': [time_steps[Tn]]
+                                                                            })], axis=1))  
+                                                                
+            # # Concatenate out list of dataframes into single catalog dataframe
+            # catalog = pd.concat(out, axis=0, ignore_index=True)
+
+        # Concatenate out list of dataframes into single catalog dataframe
+        catalog = pd.concat(out, axis=0, ignore_index=True)
+
+        if len(catalog) == 0:
+            raise ValueError(f"Requested Time not found in {set(catalog['duration'])}")
+    
+    # space XY
+    if AOI is None:
+            catalog["X"]    = "[0:1:" + (catalog['ncols'] - 1).astype(int).astype(str) + "]"
+            catalog["Y"]    = "[0:1:" + (catalog['nrows'] - 1).astype(int).astype(str) + "]"
+    else: 
+            # if AOI is given, filter out rows not in AOI bounding box
+            out = []
+
+            # catalog = find_intersects(
+            # 	catalog = catalog,
+            # 	AOI     = AOI
+            # 	)
+
+            # catalog length to track progress
+            n = len(catalog)
+
+            # loop over catalog and filter out rows not in AOI bounding box
+            for i in range(len(catalog)):
+                
+                # print messages if verbose is True
+                if verbose: 
+                    print(f'Filtering out rows not in AOI bounding box: ({i+1}/{n})')
+                
+                # make a bounding box from the catalog row
+                cat_box = utils.make_ext(catalog.iloc[i])
+
+                # make a bounding box from the AOI and reproject to catalog crs
+                aoi_box = AOI.to_crs(catalog["crs"].iloc[0])['geometry'][0].bounds
+
+                # try to intersect the bounding boxes, if it fails append None to out list
+                try:
+                    out.append(shapely.box(*aoi_box).intersection(cat_box))
+                except Exception as e:
+                    out.append(None)
+            # out = Parallel(n_jobs=-1)(delayed(go_get_dap_data) (dap_data.iloc[i].to_dict()) for i in range(len(dap_data)))
+            # find the indices of the None values in out and remove the corresponding rows from catalog
+            drops = [i for i, x in enumerate(out) if x is None]
+        
+            # drop rows from catalog and remove None values from out list
+            if drops:
+                catalog = catalog.drop(drops)
+                out     = [x for x in out if x is not None]
+
+            # catalog length to track progress
+            n = len(catalog)
+
+            # loop over each row and do X/Y coord mapping
+            for i in range(len(catalog)):
+                # print messages if verbose is True
+                if verbose: 
+                    print(f'Mapping X/Y coords: ({i+1}/{n})')
+
+                X_coords = np.linspace(catalog.iloc[i, catalog.columns.get_loc('X1')], catalog.iloc[i, catalog.columns.get_loc('Xn')], num = int(catalog.iloc[i, catalog.columns.get_loc('ncols')]))
+                
+                Y_coords = np.linspace(catalog.iloc[i, catalog.columns.get_loc('Y1')], catalog.iloc[i, catalog.columns.get_loc('Yn')],  num = int(catalog.iloc[i, catalog.columns.get_loc('nrows')]))
+            
+                ys = [np.argmin(np.abs(Y_coords - out[i].bounds[1])), np.argmin(np.abs(Y_coords - out[i].bounds[3]))]
+                xs = [np.argmin(np.abs(X_coords - out[i].bounds[0])), np.argmin(np.abs(X_coords - out[i].bounds[2]))]
+                
+                catalog.loc[i, 'Y'] = f"[{':1:'.join(map(str, sorted(ys)))}]"
+                catalog.loc[i, 'X'] = f"[{':1:'.join(map(str, sorted(xs)))}]"
+
+                catalog.at[i, 'X1'] = min(X_coords[[i + 1 for i in xs]])
+                catalog.at[i, 'Xn'] = max(X_coords[[i + 1 for i in xs]])
+                catalog.at[i, 'Y1'] = min(Y_coords[[i + 1 for i in ys]])
+                catalog.at[i, 'Yn'] = max(Y_coords[[i + 1 for i in ys]])
+                catalog.at[i, 'ncols'] = abs(np.diff(xs))[0] + 1
+                catalog.at[i, 'nrows'] = abs(np.diff(ys))[0] + 1
+    
+    # DIMENSION ORDER STRINGS
+    first  = catalog['dim_order'].str[0].fillna('T').values[0]
+    second = catalog['dim_order'].str[1].fillna('Y').values[0]
+    third  = catalog['dim_order'].str[2].fillna('X').values[0]
+
+    # properly format URL string for tiled data
+    if catalog['tiled'].str.contains('XY').any():
+        catalog['URL'] = catalog['URL'] + '?' + catalog['varname'] + catalog[first] + catalog[second] + catalog[third]
+    else:
+        catalog['URL'] = catalog['URL'] + '?' + catalog['varname'] + catalog[first] + catalog[second] + catalog[third]
+    
+    # check varname
+    if varname is not None:
+        # check if varname is a str, convert to list if so
+        if isinstance(varname, str):
+            varname = [varname]
+        if varname not in catalog['varname'].unique() and varname not in catalog['variable'].unique():
+            var_list = "\t > ".join(catalog['varname'].unique())
+            raise ValueError(f"variable(s) in resource include:\n\t> {var_list}")
+        
+        catalog['varname'] == varname
+        catalog =  catalog.query("varname == @varname")
+
+    # replace NaN values with None
+    catalog = catalog.replace({np.nan: "NA"})
+
+    # TODO: look into what this does, keep commented out for now
+    # catalog["X"] = None
+    # catalog["Y"] = None
+    # catalog["T"] = None
+
+    return catalog
+
+def dap(
+        URL         = None,
+        catalog     = None,
+        AOI         = None,
+        startDate   = None,
+        endDate     = None,
+        varname     = None,
+        grid        = None,
+        start       = None,
+        end         = None,
+        toptobottom = False,
+        dopar       = True,
+        verbose     = False
+        ):
+        
+        """Get data from a DAP server"""
+
+        if not isinstance(toptobottom, bool):
+
+            # print("Checking if all toptobottom values are Nan...")
+
+            # convert to float to check for nan
+            nan_chk = toptobottom.astype(float)
+
+            # if all toptobottom values are Nan, then make toptobottom False 
+            if np.isnan(np.sum(nan_chk)):
+
+                # print("--> setting toptobottom to False")
+                toptobottom = False
+
+        # else:
+        # 	print("toptobottom is already a boolean")
+        # 	print(f"toptobottom = {toptobottom}")
+
+        # check to make sure URL or catalog is provided
+        if URL is None and catalog is None:
+            raise ValueError("URL or catalog must be provided")
+        
+
+        # check if a single string, if so, make a list of string
+        if isinstance(URL, str):
+            URL = [URL]
+
+        # if URL is None then only use catalog URL column
+        if URL is None:
+            URL = catalog.URL.values.tolist()
+
+        else:
+            # convert Numpy array to list
+            url_lst = catalog.URL.values.tolist()
+
+            # extend list with URL
+            url_lst.extend(URL)
+
+            # set URL to list of URLS
+            URL = url_lst
+
+        # check if "vrt" or "tif" in URL list, or if "vsi" in all of URL list
+        if any([utils.getExtension(i) in ['vrt', "tif"] for i in URL]) or all(["vsi" in i for i in URL]):
+
+            if verbose:
+                print("Getting VRT/TIF data")
+                
+            # get the vrt catalog features for each URL
+            vrt_data = vrt_crop_get(
+                URL         = URL,
+                catalog     = catalog,
+                AOI         = AOI,
+                grid        = grid,
+                varname     = varname,
+                start       = start,
+                end         = end,
+                toptobottom = toptobottom,
+                verbose     = False
+                )
+            
+            # # get the vrt catalog features for each URL
+            # vrt_data = vrt_crop_get2(
+            #     URL         = URL,
+            #     catalog     = catalog,
+            #     AOI         = AOI,
+            #     grid        = grid,
+            #     varname     = varname,
+            #     start       = start,
+            #     end         = end,
+            #     toptobottom = toptobottom,
+            #     verbose     = verbose
+            #     )
+            
+            return vrt_data
+
+        else:
+            if verbose:
+                print("Getting DAP data")
+
+            # get the dap catalog features for each URL
+            dap_data = dap_crop(
+                URL       = URL,
+                catalog   = catalog,
+                AOI       = AOI,
+                startDate = startDate,
+                endDate   = endDate,
+                varname   = varname,
+                verbose   = False
+                )
+            
+            # if dopar:
+            #     if verbose:
+            #         print("Getting DAP data in parallel")
+            # else:
+            #     if verbose:
+            #         print("Getting DAP data in serial")
+
+            # get dap data
+            dap_data = dap_get(
+                dap_data = dap_data,
+                dopar    = dopar,
+                verbose  = False
+                )
+            
+            return dap_data
+        
+def match_args(func, *args, **kwargs):
+
+    """Match default arguments for a function.
+
+    This function takes a function and a variable number of positional and keyword arguments.
+    It matches the provided arguments with the default arguments of the function signature
+    and returns a dictionary containing the matched arguments.
+
+    Args:
+        func (callable): The function for which arguments need to be matched.
+        *args: Positional arguments that need to be matched with function parameters.
+        **kwargs: Keyword arguments that need to be matched with function parameters.
+
+    Returns:
+        dict: A dictionary containing the matched arguments as key-value pairs.
+
+    """
+    sig = inspect.signature(func)
+    matched_args = {}
+    for k, v in sig.parameters.items():
+            if k in kwargs:
+                    matched_args[k] = kwargs[k]
+            elif args:
+                    matched_args[k] = args[0]
+                    args = args[1:]
+            else:
+                    matched_args[k] = v.default
+    return matched_args
+
+def climatepy_dap(*args, verbose = False, **kwargs):
+
+        """ClimatePy DAP (DAP).
+        
+        This is an internal function that works to take varied argument inputs and appropriatly match 
+        them to climatepy_filter() and dap_crop() functions. 
+        Args:
+            *args: Positional arguments to be matched with parameters of `climatepy_filter` and `dap_crop`.
+            verbose (bool, optional): Whether to print verbose output during DAP operations. Defaults to False.
+            **kwargs: Keyword arguments to be matched with parameters of `climatepy_filter` and `dap_crop`.
+
+        Returns:
+            dict: A dictionary containing the matched arguments for DAP operations.
+
+        """
+
+        # get matching arguments for climatepy_filter function
+        matches1            = match_args(climatepy_filter.climatepy_filter, *args, **kwargs)
+
+        # get catalog from climatepy_filter
+        x = climatepy_filter.climatepy_filter(**matches1)
+
+        # add catalog to list of arguments that'll be passed to dap
+        matches1['catalog'] = x
+
+        # matches1['verbose'] = True
+        matches1['verbose'] = verbose
+        matches1['varname'] = None
+
+        # match arguments for dap_crop function
+        matches2 = match_args(dap_crop, *args, **kwargs)
+
+        # get matching arguments in climatepy_filter and dap_crop
+        dap_matches = {k: matches1[k] for k in matches1 if k in matches2}
+
+        if verbose: 
+            print("dap_matches: ", dap_matches)
+
+        return dap_matches
+
+def var_to_da(var, dap_row):
+    """Converts a variable to an xarray DataArray with coordinate reference system (CRS).
+
+    Args:
+        var (numpy.ndarray): The variable to be converted to a DataArray.
+        dap_row (pandas.Series): A pandas Series containing metadata information.
+
+    Returns:
+        xarray.DataArray: The variable converted to a DataArray with CRS included.
+
+    """
+
+    # var = get_data(dap_row)
+    # dap_row = dap_row
+
+    # dates = pd.to_datetime(dates)
+    dates = pd.date_range(
+        start   = dap_row['startDate'], 
+        end     = dap_row['endDate'], 
+        periods = dap_row['Tdim']
+        )
+
+    # concatenate variable name with date and model info
+    name = dap_row['variable'] + '_' + dates.strftime('%Y-%m-%d-%H-%M-%S') + '_' + dap_row['model'] + '_' + dap_row['ensemble'] + '_' + dap_row['scenario']
+    name = name.str.replace('_NA', '', regex=False)
+    name = name.str.replace('_na', '', regex=False)
+
+    # extract variable name
+    vars = dap_row['variable']
+
+    # if variable name is NA, use varname
+    if len(vars) == 0:
+        vars = dap_row['varname']
+
+    # clean up timeseries names
+    names_ts = "_".join([vars, dap_row["model"], dap_row["ensemble"], dap_row["scenario"]])
+    names_ts = names_ts.replace("_NA", "")
+    names_ts = names_ts.replace("_na", "")
+    names_ts = names_ts.replace("__", "_")
+    names_ts = names_ts.rstrip("_")
+
+    # if dap_row has 1 column and 1 row, or 1 key/value
+    if len(dap_row.keys()) == 1 and len(dap_row.values()) == 1:
+        # reshape var into a 2D array
+        var_2d = var.reshape((len(dates), -1))
+
+        # create a dictionary of column names and values
+        var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
+        var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
+
+        # create a DataFrame with dates and var_dict as columns
+        df = pd.DataFrame({'date': dates, **var_dict})
+
+    # x resolution
+    resx = (dap_row['Xn'] - dap_row['X1'])/(dap_row['ncols'] - 1)
+
+    # y resolution
+    resy = (dap_row['Yn'] - dap_row['Y1'])/(dap_row['nrows'] - 1)
+
+    xmin = dap_row['X1'] - 0.5 * resx
+    xmax = dap_row['Xn'] + 0.5 * resx
+    ymin = dap_row['Y1'] - 0.5 * resy
+    ymax = dap_row['Yn'] + 0.5 * resy
+
+    # expand dimensions of 'var' if it's a 2D array
+    if var.ndim == 2:
+        var = np.expand_dims(var, axis=-1)
+    
+    # check if size of first dimension of 'var' is equals number of rows in 'dap'
+    if var.shape[2] != dap_row["nrows"]:
+        # transpose the first two dimensions of 'var' if not in correct order
+        var = var.transpose(dap_row["Y_name"], dap_row["X_name"], dap_row["T_name"])
+        # var2 = var.transpose(dap_row["T_name"], dap_row["X_name"],  dap_row["Y_name"])
+    
+    # Create the DataArray with the CRS included
+    r = xr.DataArray(
+        var,
+        coords = {
+            'y': -1*np.linspace(ymin, ymax, dap_row['nrows'], endpoint=False),
+            'x': np.linspace(xmin, xmax, dap_row['ncols'], endpoint=False),
+            'time': dates,
+            'crs': dap_row['crs']
+        },
+        dims=['y', 'x', 'time']
+        )
+
+    # if toptobottom is True, flip the data vertically
+    if dap_row['toptobottom']:
+
+        # vertically flip each 2D array
+        flipped_data = np.flip(r.values, axis=0)
+        # flipped_data = np.flipud(r.values)
+
+        # create new xarray DataArray from flipped NumPy array
+        r = xr.DataArray(
+            flipped_data,
+            dims   = ('y', 'x', 'time'),
+            coords = {'y': r.y, 'x': r.x, 'time': r.time}
+            )
+
+    # set the name attribute of the DataArray
+    r = r.assign_coords(time=name)
+
+    return r
+
+def get_data(dap_row):
+    """Internal function for retrieving data from a DAP (Data Access Protocol) source.
+
+    Args:
+        dap_row (pandas.Series): A pandas Series containing metadata information.
+
+    Returns:
+        xarray.DataArray: The retrieved variable data.
+
+    """
+
+    ds = xr.open_dataset(f"{dap_row['URL']}#fillmismatch")
+
+    var = ds[dap_row['varname']]
+
+    ds.close()
+
+    return var
+
+def go_get_dap_data(dap_row):
+
+    """Internal function for retrieving DAP (Data Access Protocol) data and converting it to a DataArray.
+
+    Args:
+        dap_row (pandas.Series): A pandas Series containing metadata information.
+
+    Returns:
+        xarray.DataArray or str: The retrieved data as a DataArray, or the original URL if an error occurred.
+
+    """
+
+    # dap_row = dap_data.iloc[i].to_dict()
+    try:
+        if "http" in dap_row["URL"]:
+            x = var_to_da(var = get_data(dap_row), dap_row = dap_row)
+        else:
+            raise Exception("dap_to_local() not avaliable, yet, dataset URL must be in http format")
+    except Exception as e:
+        return dap_row["URL"]
+    
+    return x
+
+def add_varname_attr(
+        out = None, 
+        dap_data = None, 
+        verbose = False
+        ):
+    
+    for da, varb in zip(out, dap_data["variable"]):
+        if verbose: 
+            print(f'Adding "variable" attribute {varb} to DataArray')
+        da.attrs["variable"] = varb
+
+    for da, varname in zip(out, dap_data["varname"]):
+        if verbose: 
+            print(f'Adding "var" attribute {varname} to DataArray')
+        da.attrs["varname"] = varname
+
+def merge_across_time(data_arrays, verbose = False):
+
+    """Merge DataArrays across time"""
+
+    if verbose:
+        print("Merging DataArrays across time")
+
+    # create a dictionary to store DataArrays for each unique variable_name
+    da_dict = {}
+
+    n = len(data_arrays)
+
+    for idx, val in enumerate(data_arrays):
+        variable_name = val.attrs.get('variable', 'unknown')
+        # print("Iterating through list of DataArrays: ", variable_name, "-", idx+1, "/", len(data_arrays), " DataArrays")
+
+        if verbose:
+            print(f"Iterating through list of DataArrays: {variable_name} - ({idx+1}/{n})")
+            # print("Iterating through list of DataArrays: ", variable_name)
+
+        if variable_name not in da_dict:
+            if verbose:
+                print("----> variable ", variable_name, "NOT IN da_dict")
+                # print("variable NOT IN da_dict adding dataarray list with key: ", variable_name)
+            da_dict[variable_name] = [val]
+        else:
+            if verbose:
+                print("----> variable ", variable_name, "IN da_dict")
+                # print("variable IN da_dict, appending data array to key: ", variable_name)
+            da_dict[variable_name].append(val)
+
+    # for da in data_arrays:
+    #     variable_name = da.attrs.get('variable_name', 'unknown')
+    #     if variable_name not in da_dict:
+    #         da_dict[variable_name] = [da]
+    #     else:
+    #         da_dict[variable_name].append(da)
+
+    # concatenate DataArrays for each unique variable_name
+    concat_da = []
+    for variable_name, da_list in da_dict.items():
+
+        if verbose:
+            print("--> concatenating time dims: ", variable_name)
+
+        # concatenate DataArrays along the time dimension
+        cda = xr.concat(da_list, dim='time')
+
+        # add variable_name as an attribute to the concatenated DataArray
+        cda.attrs['variable'] = variable_name
+
+        # add the concatenated DataArray to the list of output DataArrays
+        concat_da.append(cda)
+
+    return concat_da
+
+def dap_get(dap_data, dopar = True, varname = None, verbose = False):
+    
+    """Get DAP resource data.
+
+    Args:
+        dap_data (pandas.DataFrame): A DataFrame containing metadata information for DAP resources.
+        dopar (bool, optional): Flag indicating whether to perform parallel execution. Defaults to True.
+        varname (str, optional): The variable name to filter the DAP resources. Defaults to None.
+        verbose (bool, optional): Flag indicating whether to print verbose output. Defaults to False.
+
+    Returns:
+        dict or xarray.DataArray: A dictionary of DataArrays or a single DataArray, representing the retrieved DAP data.
+
+    Raises:
+        ValueError: If the provided varname is not found in the DAP resources.
+
+    """
+    
+    # check if varname is in dap_data
+    if varname is not None:
+        if varname not in dap_data["varname"].values and varname not in dap_data["variable"].values:
+        # if varname not in dap_data['varname'].unique() and varname not in dap_data['variable'].unique():
+            errstr = "\t > ".join(dap_data["varname"].unique())
+            raise ValueError(f'variable(s) in resource include:\n\t > {errstr}' )
+        
+        # filter done dap_data to only include varname if varname is None
+        dap_data = dap_data[
+            (dap_data.get("varname", False) == varname) |
+            (dap_data.get("variable", False) == varname)
+            ]
+        
+    if dopar:
+        # make go_get_dap_data calls in parallel
+        out = Parallel(n_jobs=-1)(delayed(go_get_dap_data) (dap_data.iloc[i].to_dict()) for i in range(len(dap_data)))
+        # out_lst = [go_get_dap_data(dap_row = dap_data.iloc[i].to_dict()) for i in range(len(dap_data))]
+    else:
+        # store output list 
+        out = []
+        # get number of rows in dap_data
+        n = len(dap_data)
+        # # next is to loop over each row in dap_data and call go_get_dap_data
+        for i in range(len(dap_data)):
+            if verbose:
+                print(f'Getting dap data: ({i+1}/{n})')
+
+            x = go_get_dap_data(dap_row = dap_data.iloc[i].to_dict())
+            out.append(x)
+    
+    # add variable name attribute to each DataArray in the output list
+    add_varname_attr(
+        out      = out,
+        dap_data = dap_data, 
+        verbose  = verbose
+        )
+    
+    # merge across time
+    out = merge_across_time(data_arrays = out, verbose = verbose)
+    
+    # concatenated_da = xr.concat(data_arrays, dim=('time', "variable_name"))
+
+    # TODO: USE THIS LIST COMPREHENSION, standard for loop is easier for debugging
+    # next is to loop over each row in dap_data and call go_get_dap_data
+    # out = [go_get_dap_data(dap_data.iloc[x].to_dict()) for x in range(len(dap_data))]
+    # out = [go_get_dap_data(dap_data.iloc[x]) for x in range(len(dap_data))]
+
+    # get data names
+    out_names = list(dict.fromkeys([name.replace("_$", "") for name in dap_data['variable'].tolist()]))
+    # out_names = list(dict.fromkeys([name.replace("_$", "") for name in dap_data['varname'].tolist()]))
+    # out_names = list(set([name.replace("_$", "") for name in dap_data["varname"]]))
+    # out_names = [name.replace("_$", "") for name in dap_data["varname"]]
+    # out_names = dap_data['varname'].str.replace('_$', '').tolist()
+
+    # put list and names into a dictionary
+    out = dict(zip(out_names, out))
+
+    # Check if first DataArray is not a SpatRaster
+    if not isinstance(out[next(iter(out))], xr.core.dataarray.DataArray):
+        if verbose:
+            print("Processing non DataArray data...")
+
+        # out = list(out.values())
+        # out = xr.merge(out, join="outer")
+        # out = reduce(lambda dtf1, dtf2: dtf1.merge(dtf2, on="date", how="outer"), out)
+
+        return out
+    
+    elif any(dap_data["tiled"].str.contains("XY")):
+        if verbose:
+            print("Processing 'XY' data...")
+
+        ll = {}
+        u = np.unique([da.units for da in out])
+
+        if len(u) == 1:
+            out = xr.combine_by_coords(out)
+            out["units"] = (["layer"], [u[0]] * len(out["layer"]))
+            ll[dap["varname"].iloc[0]] = out
+            out = ll
+
+            return out
+        else:
+            # out = dict(zip(out_names, out))
+            return out
+
+    elif any(dap_data["tiled"] == "T"):
+
+        print("Processing 'T' data...")
+
+        # out = xr.concat(out, dim="time").sortby("time")
+        return out
+    else:
+        if verbose:
+            print("Processing as normal...")
+        
+        return out
+
+    return out
+
+def var_to_rast(var, dap_row):
+    """
+    Convert a variable to a raster format.
+
+    Args:
+        var (numpy.ndarray): The variable data to convert.
+        dap_row (pandas.Series): A row from the Data Access Protocol (DAP) climate catalog pandas dataframe containing metadata information.
+
+    Returns:
+        xr.DataArray: The converted variable as a DataArray.
+
+    """
+    
+    # dates = pd.to_datetime(dates)
+    dates = pd.date_range(
+        start   = dap_row['startDate'], 
+        end     = dap_row['endDate'], 
+        periods = dap_row['Tdim']
+        )
+
+    # concatenate variable name with date and model info
+    name = dap_row['variable'] + '_' + dates.strftime('%Y-%m-%d-%H-%M-%S') + '_' + dap_row['model'] + '_' + dap_row['ensemble'] + '_' + dap_row['scenario']
+    name = name.str.replace('_NA', '', regex=False)
+
+    # extract variable name
+    vars = dap_row['variable']
+
+    # if variable name is NA, use varname
+    if len(vars) == 0:
+        vars = dap_row['varname']
+
+    # clean up timeseries names
+    names_ts = "_".join([vars, dap_row["model"], dap_row["ensemble"], dap_row["scenario"]])
+    names_ts = names_ts.replace("_NA", "")
+    names_ts = names_ts.replace("__", "_")
+    names_ts = names_ts.rstrip("_")
+
+    # if dap_row has 1 column and 1 row, or 1 key/value
+    if len(dap_row.keys()) == 1 and len(dap_row.values()) == 1:
+        # reshape var into a 2D array
+        var_2d = var.reshape((len(dates), -1))
+
+        # create a dictionary of column names and values
+        var_dict = {f'var_{i}': var_2d[:, i] for i in range(var_2d.shape[1])}
+        var_dict = {key.replace("var_", f'{names_ts}_'): var_dict[key] for key in var_dict.keys()}
+
+        # create a DataFrame with dates and var_dict as columns
+        df = pd.DataFrame({'date': dates, **var_dict})
+
+    # x resolution
+    resx = (dap_row['Xn'] - dap_row['X1'])/(dap_row['ncols'] - 1)
+
+    # y resolution
+    resy = (dap_row['Yn'] - dap_row['Y1'])/(dap_row['nrows'] - 1)
+
+    xmin = dap_row['X1'] - 0.5 * resx
+    xmax = dap_row['Xn'] + 0.5 * resx
+    ymin = dap_row['Y1'] - 0.5 * resy
+    ymax = dap_row['Yn'] + 0.5 * resy
+
+    # expand dimensions of 'var' if it's a 2D array
+    if var.ndim == 2:
+        var = np.expand_dims(var, axis=-1)
+
+    # check if size of first dimension of 'var' is equals number of rows in 'dap'
+    if var.shape[2] != dap_row["nrows"]:
+        # transpose the first two dimensions of 'var' if not in correct order
+        var = var.transpose(dap_row["Y_name"], dap_row["X_name"], dap_row["T_name"])
+        # var2 = var.transpose(dap_row["T_name"], dap_row["X_name"],  dap_row["Y_name"])
+
+    # Create the DataArray with the CRS included
+    r = xr.DataArray(
+        var,
+        coords = {
+            'y': -1*np.linspace(ymin, ymax, dap_row['nrows'], endpoint=False),
+            'x': np.linspace(xmin, xmax, dap_row['ncols'], endpoint=False),
+            'time': dates,
+            'crs': dap_row['crs']
+        },
+        dims=['y', 'x', 'time']
+        )
+
+    # if toptobottom is True, flip the data vertically
+    if dap_row['toptobottom']:
+
+        # vertically flip each 2D array
+        flipped_data = np.flip(r.values, axis=1)
+
+        # create new xarray DataArray from flipped NumPy array
+        r = xr.DataArray(
+            flipped_data,
+            dims   = ('y', 'x', 'time'),
+            coords = {'y': r.y, 'x': r.x, 'time': r.time}
+            )
+        
+    # set the name attribute of the DataArray
+    r = r.assign_coords(time=name)
+
+    return r
+
+def do_dap(catalog, AOI, varname, verbose = False):
+        dap_data = dap(
+            catalog = catalog,
+            AOI     = AOI,
+            verbose = verbose
+            )
+        return dap_data[varname]
+
+def repeat_durations(start_date, end_date, repeat_count):
+    """Repeat durations between start_date and end_date.
+
+    Args:
+        start_date (str or datetime): Start date of the duration.
+        end_date (str or datetime): End date of the duration.
+        repeat_count (int): Number of times to repeat the durations.
+
+    Returns:
+        list: List of repeated durations in the format 'YYYY-MM-DD/YYYY-MM-DD'.
+    """
+    date_list = pd.date_range(start=start_date, end=end_date, freq='D').tolist()
+    repeated_dates = []
+    for date in date_list:
+        for i in range(repeat_count):
+            repeated_dates.append(date)
+    durs = [f'{i.strftime("%Y-%m-%d")}/{i.strftime("%Y-%m-%d")}' for i in repeated_dates]
+    return durs
+
+def get_prism_daily(AOI, varname, startDate, endDate, verbose = False):
+
+    """Retrieve PRISM daily climate data.
+
+    Args:
+        AOI (str): Area of interest.
+        varname (str): Variable name.
+        startDate (str or datetime): Start date of the data.
+        endDate (str or datetime): End date of the data.
+        verbose (bool): Verbosity flag.
+
+    Returns:
+        dict: Dictionary containing the retrieved climate data.
+    """
+        
+    # collect raw meta data
+    raw = climatepy_filter.climatepy_filter(
+        id        = "prism_daily", 
+        AOI       = AOI, 
+        varname   = varname,
+        startDate = startDate,
+        endDate   = endDate
+    )
+
+    if endDate is None:
+        endDate = startDate
+
+    # collect varname in correct order
+    varname = raw.varname.unique().tolist()
+
+    # for i in range(len(varname)):
+    #     # make dates for each variable
+    #     pd.date_range(start=startDate, end=endDate, freq='D').tolist()
+    # convert to datetime objects and create date range
+    dates = pd.date_range(start=startDate, end=endDate, freq='D').tolist()
+
+    # create new DataFrame with xx column for each date in dates
+    out = [raw.assign(x=date) for date in dates]
+    
+    # concatenate all DataFrames into a single DataFrame
+    out = pd.concat(out, ignore_index=True)
+
+    # add YYYY column
+    out = out.assign(YYYY=out['x'].apply(lambda x: x.year))
+
+    # convert datetime column to YYYY-MM-DD string format
+    out['x'] = out['x'].dt.strftime('%Y-%m-%d')
+
+    # create a YYYYMMDD column from string date
+    out = out.assign(YYYYMMDD=out['x'].apply(lambda x: x.replace("-", "")))
+
+    # define lambda function to replace substrings in URL column
+    replace_values = lambda x: x['URL'].replace('{YYYY}', str(x['YYYY'])).replace('{YYYYMMDD}', str(x['YYYYMMDD']))
+
+    # apply lambda function to DataFrame
+    out['URL'] = out.apply(replace_values, axis=1)
+
+    # add duration column
+    out['duration'] = repeat_durations(startDate, endDate, len(varname))
+    # out['duration'] = [f'{i.strftime("%Y-%m-%d")}/{i.strftime("%Y-%m-%d")}' for i in dates]
+
+    # from joblib import Parallel, delayed, parallel_backend
+    out_lst = Parallel(n_jobs=-1)(delayed(do_dap) (catalog = out.iloc[[i]], 
+                                                AOI  = AOI,
+                                                varname = out.varname.iloc[i], 
+                                                verbose = False
+                                                ) for i in range(len(out)))
+    # out_lst = []
+    # for i in range(len(out)):
+        
+    #     dap_data = do_dap(
+    #         catalog = out.iloc[[i]],
+    #         AOI     = AOI,
+    #         varname = out.varname.iloc[i],
+    #         verbose = verbose
+    #     )
+        # out_lst.append(dap_data)
+        # out_lst.append(dap_data[out.varname.iloc[i]])
+    
+    out_lst = merge_across_time(out_lst)
+
+    # type(out_lst[0])
+    # get data names
+    out_names = list(dict.fromkeys([name.replace("_$", "") for name in out['variable'].tolist()]))
+
+    # put list and names into a dictionary
+    out = dict(zip(out_names, out_lst))
+
+    return out
+
+def get_nodata(dtype):
+    """Returns the NoData value based on the data type.
+
+    Args:
+        dtype (str): The data type string.
+
+    Returns:
+        The NoData value corresponding to the data type. If the data type is 'int', returns 0. If the data type is 'float',
+        returns np.nan. If the data type is 'uint', returns 0. If the data type is 'complex', returns 0 + 0j. If the data
+        type is 'bool', returns False. For any other data type, returns None.
+    """
+
+    if "int" in dtype:
+        return 0
+    elif "float" in dtype:
+        # return 0.0 if dtype == "float32" or dtype == "float64" else np.nan
+        return np.nan
+    elif "uint" in dtype:
+        return 0
+    elif "complex" in dtype:
+        return 0 + 0j
+    elif "bool" in dtype:
+        return False
+    else:
+        return None
+    
+
+def crop_vrt2(urls, AOI, verbose = False):
+
+    """Crop a VRT to an AOI"""
+
+    # Function for opening a single VRT file with rasterio
+    def crop_vrt_for_url(url, AOI, verbose):
+        
+        with rio.open(url) as src:
+            if verbose: 
+                print('Source tags:', src.tags(1))
+                print("Source desc: ", src.descriptions)
+                print("Source profile: ", src.profile)
+
+            # Reproject the geometry to the CRS of the DataArray
+            AOIv = AOI.to_crs(src.crs, inplace=False)
+
+            # Get the bounding box of your AOI shape
+            bbox = AOIv.geometry.total_bounds
+
+            # Create a polygon object representing the bounding box
+            bounding_box = shapely.geometry.box(bbox[0], bbox[1], bbox[2], bbox[3])
+
+            if verbose:
+                print(" Cropping VRT to bounding box...")
+
+            # check data types and get nodata value
+            dtype   = src.profile['dtype']
+            no_data = get_nodata(dtype)
+
+            print("dtype: ", dtype)
+            print("nodata: ", no_data)
+
+            # out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, invert = False)
+            out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, nodata = no_data, invert = False)
+            out_meta = src.meta
+            out_tags = src.tags(1)
+
+            # if nodata in out_meta, replace nodata value with value used as nodata
+            if 'nodata' in out_meta:
+                out_meta['nodata'] = no_data
+
+            # if nodata in out_tags, replace nodata value with value used as nodata
+            if 'nodata' in out_tags:
+                out_tags['nodata'] = no_data
+
+            # out_image, out_transform = rio.mask.mask(src, AOIv.geometry, crop=True, nodata=np.nan, invert = False)
+            # out_meta = src.meta
+            
+            # close the dataset
+            src.close()
+
+        if out_image.ndim == 3:
+            out_image = out_image.squeeze()
+
+        # bb = AOI.geometry.total_bounds
+        # rio.windows.from_bounds(*bb, out_transform)
+
+        # get height and width of image
+        height = out_image.shape[0]
+        width = out_image.shape[1]
+
+        # get x and y width height indices
+        x_indices = np.arange(width)
+        y_indices = np.arange(height)
+
+        # create meshgrid
+        x_coords, y_coords = np.meshgrid(x_indices, y_indices)
+
+        # get affine transform for coordinates
+        x_coords, y_coords = rio.transform.xy(out_transform, y_coords, x_coords)
+
+        # stack the arrays along a new dimension
+        coords = np.stack((x_coords, y_coords), axis=-1)
+
+        # x and y stacks
+        xn = np.stack((x_coords), axis=-1)
+        yn = np.stack((y_coords), axis=-1)
+
+        # get min and max of x and y
+        xmin = xn.min()
+        xmax = xn.max()
+        ymin = yn.min()
+        ymax = yn.max()
+
+        # # GET CRS
+        # crs = out_meta['crs']
+
+        # create DataArray
+        r = xr.DataArray(
+            out_image,
+            coords={
+                'y': -1*np.linspace(ymin, ymax, height, endpoint=False),
+                'x': np.linspace(xmin, xmax, width, endpoint=False),
+            },
+            dims=['y', 'x']
+        )
+
+        # add tags to attributes of data array
+        for key, value in out_tags.items():
+            r.attrs[key] = value
+
+        # add tags to attributes of data array
+        for key, value in out_meta.items():
+            r.attrs[key] = value
+
+        return r
+    
+
+    # tmp = crop_vrt_for_url(urls[1], AOI, verbose = True)
+    results = Parallel(n_jobs=-1)(delayed(crop_vrt_for_url) (url = i,
+                                            AOI  = AOI,
+                                            verbose = False
+                                            ) for i in urls)
+    
+    return results
+
+def crop_vrt(urls, AOI, verbose = False):
+
+    """Crop a VRT to an AOI"""
+
+    # make empty list to store dataarrays
+    da_lst = []
+
+    # loop over each url
+    for url in urls:
+        with rio.open(url) as src:
+            if verbose: 
+                print('Source tags:', src.tags(1))
+                print("Source desc: ", src.descriptions)
+                print("Source profile: ", src.profile)
+
+            # Reproject the geometry to the CRS of the DataArray
+            AOIv = AOI.to_crs(src.crs, inplace=False)
+
+            # Get the bounding box of your AOI shape
+            bbox = AOIv.geometry.total_bounds
+
+            # Create a polygon object representing the bounding box
+            bounding_box = shapely.geometry.box(bbox[0], bbox[1], bbox[2], bbox[3])
+
+            if verbose:
+                print(" Cropping VRT to bounding box...")
+
+            # check data types and get nodata value
+            dtype   = src.profile['dtype']
+            no_data = get_nodata(dtype)
+
+            print("dtype: ", dtype)
+            print("nodata: ", no_data)
+
+            # out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, invert = False)
+            out_image, out_transform = rio.mask.mask(src, [bounding_box], crop=True, nodata = no_data, invert = False)
+            out_meta = src.meta
+            out_tags = src.tags(1)
+
+            # if nodata in out_meta, replace nodata value with value used as nodata
+            if 'nodata' in out_meta:
+                out_meta['nodata'] = no_data
+
+            # if nodata in out_tags, replace nodata value with value used as nodata
+            if 'nodata' in out_tags:
+                out_tags['nodata'] = no_data
+
+            # out_image, out_transform = rio.mask.mask(src, AOIv.geometry, crop=True, nodata=np.nan, invert = False)
+            # out_meta = src.meta
+            
+            # close the dataset
+            src.close()
+
+        if out_image.ndim == 3:
+            out_image = out_image.squeeze()
+
+        # bb = AOI.geometry.total_bounds
+        # rio.windows.from_bounds(*bb, out_transform)
+
+        # get height and width of image
+        height = out_image.shape[0]
+        width = out_image.shape[1]
+
+        # get x and y width height indices
+        x_indices = np.arange(width)
+        y_indices = np.arange(height)
+
+        # create meshgrid
+        x_coords, y_coords = np.meshgrid(x_indices, y_indices)
+
+        # get affine transform for coordinates
+        x_coords, y_coords = rio.transform.xy(out_transform, y_coords, x_coords)
+
+        # stack the arrays along a new dimension
+        coords = np.stack((x_coords, y_coords), axis=-1)
+
+        # x and y stacks
+        xn = np.stack((x_coords), axis=-1)
+        yn = np.stack((y_coords), axis=-1)
+
+        # get min and max of x and y
+        xmin = xn.min()
+        xmax = xn.max()
+        ymin = yn.min()
+        ymax = yn.max()
+
+        # # GET CRS
+        # crs = out_meta['crs']
+
+        # create DataArray
+        r = xr.DataArray(
+            out_image,
+            coords={
+                'y': -1*np.linspace(ymin, ymax, height, endpoint=False),
+                'x': np.linspace(xmin, xmax, width, endpoint=False),
+            },
+            dims=['y', 'x']
+        )
+
+        # add tags to attributes of data array
+        for key, value in out_tags.items():
+            r.attrs[key] = value
+
+        # add tags to attributes of data array
+        for key, value in out_meta.items():
+            r.attrs[key] = value
+        # [r.attrs.update({key: value}) for key, value in out_tags.items()]    
+
+        da_lst.append(r)
+        # dataarrays[url] = r
+
+    return da_lst
+
+def vrt_crop_get(
+        URL         = None, 
+        catalog     = None, 
+        AOI         = None, 
+        grid        = None,
+        varname     = None, 
+        start       = None, 
+        end         = None, 
+        toptobottom = False, 
+        verbose     = False
+        ):
+    
+#     """
+#     Crop and process VRT data.
+
+#     Args:
+#         URL (str or list, optional): The URL(s) of the VRT file(s) to open. If not provided, it is extracted from the catalog.
+#         catalog (object, optional): The catalog object containing the URL(s) of the VRT file(s). Required if URL is not provided.
+#         AOI (geopandas.GeoDataFrame, optional): The Area of Interest polygon to crop the VRT data to.
+#         grid (object, optional): The grid object defining the extent and CRS for cropping and reprojection.
+#         varname (str, optional): The name of the variable to select from the VRT data.
+#         start (int, optional): The start index for subsetting bands in the VRT data.
+#         end (int, optional): The end index for subsetting bands in the VRT data.
+#         toptobottom (bool, optional): Whether to flip the data vertically.
+#         verbose (bool, optional): Whether to print informative messages during processing. Default is False
+
+#     Returns:
+#         xr.DataArray: The cropped and processed VRT data.
+
+#     """
+
+    if URL is None:
+        URL = catalog.URL.to_list()
+
+    if verbose:
+        print("Opening VRT from URL: ", URL)
+ 
+    # Area of interest
+    vrts = crop_vrt(urls = URL, AOI = AOI, verbose = verbose)
+
+    # vrts2 = Parallel(n_jobs=-1)(delayed(crop_vrt) (urls = [i],
+    #                                     AOI  = AOI,
+    #                                     verbose = False
+    #                                     ) for i in URL)
+
+    # check if data needs to be vertically flipped
+    for idx, val in enumerate(catalog['toptobottom']):
+
+        if verbose:
+            print("idx:", idx, "val: ",val)
+
+        if val and not np.isnan(val):
+
+            if verbose:
+                print("Flipping data vertically")
+            # vertically flip each 2D array
+            flipped_data = np.flip(vrts[idx].values, axis=0)
+
+            # stash tags
+            tags = vrts[idx].attrs
+
+            # create new xarray DataArray from flipped NumPy array
+            vrts[idx] = xr.DataArray(
+                flipped_data,
+                dims   = ('y', 'x'),
+                coords = {'y': vrts[idx].y, 'x': vrts[idx].x}
+                )
+            
+            # add tags back to flipped DataArray
+            vrts[idx].attrs = tags
+
+        else:
+            if verbose:
+                print("Not flipping data vertically")
+            # vrts[idx] = np.flip(vrts[idx], axis=0)
+
+    # create dictionary of DataArrays
+    vrts = dict(zip(catalog['variable'], vrts))
+
+    return vrts
+
+def parse_date(duration, interval):
+        """Parse the date range based on the duration and interval.
+
+        Args:
+            duration (str): The duration string in the format "start_date/end_date".
+            interval (str): The interval string specifying the time unit.
+        
+        Returns:
+            pd.DatetimeIndex: A pandas DatetimeIndex representing the parsed date range.
+        """
+        
+        # split duration string
+        d = duration.split("/")
+        
+        # if end date is "..", set it to today's date
+        if d[1] == "..":
+                d[1] = datetime.now().strftime("%Y-%m-%d")
+
+        # if interval in ["1 month", "1 months"]:
+        if any(keyword in interval for keyword in ["1 month", "1 months", "monthly"]):
+        # if any(keyword in interval for keyword in ["1 month", "1 months", "31 days", "monthly"]):
+                d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-01")
+
+        # if interval in ["hour", "hours"]:
+        if any(keyword in interval for keyword in ["hour", "hours"]):
+                d[0] = datetime.strptime(d[0], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
+                d[1] = datetime.strptime(d[1], "%Y-%m-%d").strftime("%Y-%m-%d %H:%M:%S")
+
+        # if interval is 31 days, change to 1 month
+        if interval in ["31 days","31.5 days"]:
+            interval = "1 month"
+
+        # if interval is 365, 365.5 days, change to 1 year
+        if interval in ["365 days","365.5 days"]:
+            interval = "1 year"
+
+        interval_map = {
+            "hour": "H",
+            "hours": "H",
+            "minute": "min",
+            "minutes": "min",
+            "second": "S",
+            "seconds": "S",
+            "month": "MS",  # Month Start
+            "months": "MS"  # Month Start
+            }
+        
+        # split interval string
+        interval_type = interval.split(" ")[-1]
+
+        # get frequency from interval_map
+        freq = interval_map.get(interval_type, interval_type[0])
+        
+        # # convert start_date and end_date to pandas Timestamp objects
+        # start_date = pd.Timestamp(d[0])
+        # end_date = pd.Timestamp(d[1])
+        # # calculate the number of days between start and end dates
+        # delta = (end_date - start_date) / (nT - 1)
+        # # generate the date range
+        # date_range = pd.date_range(start=start_date, end=end_date, freq=str(int(delta.days))+'D')
+
+        return pd.date_range(start=d[0], end=d[1], freq=freq)
+
+# def parse_date2(duration, nT):
+    # duration = catalog["duration"].iloc[i]
+    # interval = catalog["interval"].iloc[i]
+    # nT = catalog["nT"].iloc[i]
+#     d = duration.split("/")
+#     if d[1] == "..":
+#         d[1] = pd.Timestamp.today().strftime("%Y-%m-%d")
+#     duration = pd.to_datetime(d[1]) - pd.to_datetime(d[0])
+#     start_date = pd.to_datetime(d[0])
+#     end_date = pd.to_datetime(d[1])
+#     duration_in_days = (end_date - start_date).days
+
+#     # calculate interval in days
+#     interval_in_days = duration_in_days / nT
+# 	interval_in_days = 31
+#     # calculate the number of days to shift the frequency
+#     days_to_shift = (start_date + pd.offsets.MonthBegin(1) - start_date).days
+    
+#     # create frequency string with the offset of days to shift
+#     freq = str(int(interval_in_days)) + 'D'
+#     freq = pd.tseries.offsets.DateOffset(days=days_to_shift) 
+#     # + pd.tseries.offsets.CustomBusinessDay(n=interval_in_days)
+#     return pd.date_range(start=start_date, end=end_date, freq=freq)
+# 	interval_in_days = duration / nT
+#     if interval_in_days >= pd.Timedelta(days=365):
+#         freq = 'AS'
+#     elif interval_in_days >= pd.Timedelta(days=30):
+#         freq = 'M'
+#     elif interval_in_days >= pd.Timedelta(days=1):
+#         freq = 'D'
+#     else:
+#         freq = 'H'
+#     return pd.date_range(start=d[0], end=d[1], freq=freq)
+
+# def parse_date2(duration, interval):
+#     d = duration.split("/")
+#     if d[1] == "..":
+#         d[1] = datetime.now().strftime("%Y-%m-%d")
+#     # Get the start and end dates
+#     start_date, end_date = map(lambda x: datetime.strptime(x, '%Y-%m-%d'), d)
+
+#     # Set the start date to the first day of the month
+#     start_date = start_date.replace(day=1)
+#     if "hour" in interval:
+#         # Truncate the start and end dates to the nearest hour
+#         start_date = start_date.replace(minute=0, second=0)
+#         end_date = end_date.replace(minute=0, second=0)
+#     # interval_map = {
+#     #     "hour": "%H",
+#     #     "hours": "%H",
+#     #     "minute": "%M",
+#     #     "minutes": "%M",
+#     #     "second": "%S",
+#     #     "seconds": "%S",
+#     #     "month": "MS",  # Month Start
+# 	# 	"months": "MS"  # Month Start
+#     # }
+#     interval_type = interval.split(" ")[-1]
+#     print("interval_type: ", interval_type)
+#     freq = interval_map.get(interval_type, interval_type[0])
+#     print("frequency date: ", freq)
+#     return pd.date_range(start=d[0], end=d[1], freq=freq)
+#     # return pd.date_range(start=start_date.strftime("%Y-%m-%d"), end=end_date.strftime("%Y-%m-%d"), freq=freq)
+# def filter_row(i, catalog, AOI):
+#     # make a bounding box from the catalog row
+#     cat_box = make_ext(catalog.iloc[i])
+#     # make a bounding box from the AOI and reproject to catalog crs
+#     aoi_box = AOI.to_crs(catalog["crs"].iloc[0])['geometry'][0].bounds
+#     # try to intersect the bounding boxes, if it fails append None to out list
+#     try:
+#         return shapely.box(*aoi_box).intersection(cat_box)
+#     except Exception as e:
+#         return None
+
+# def vrt_crop_get2(
+#         URL         = None, 
+#         catalog     = None, 
+#         AOI         = None, 
+#         grid        = None,
+#         varname     = None, 
+#         start       = None, 
+#         end         = None, 
+#         toptobottom = False, 
+#         verbose     = False
+#         ):
+    
+#     """
+#     Crop and process VRT data.
+
+#     Args:
+#         URL (str or list, optional): The URL(s) of the VRT file(s) to open. If not provided, it is extracted from the catalog.
+#         catalog (object, optional): The catalog object containing the URL(s) of the VRT file(s). Required if URL is not provided.
+#         AOI (geopandas.GeoDataFrame, optional): The Area of Interest polygon to crop the VRT data to.
+#         grid (object, optional): The grid object defining the extent and CRS for cropping and reprojection.
+#         varname (str, optional): The name of the variable to select from the VRT data.
+#         start (int, optional): The start index for subsetting bands in the VRT data.
+#         end (int, optional): The end index for subsetting bands in the VRT data.
+#         toptobottom (bool, optional): Whether to flip the data vertically.
+#         verbose (bool, optional): Whether to print informative messages during processing.
+
+#     Returns:
+#         xr.DataArray: The cropped and processed VRT data.
+
+#     """
+
+#     if URL is None:
+#         URL = catalog.URL.to_list()
+
+#     if verbose:
+#         print("Opening VRT from URL: ", URL)
+
+#     # Read in each file as a separate DataArray and put them in a list
+#     vrts = [xr.open_rasterio(url) for url in URL]
+
+#     # Concatenate the DataArrays along the band dimension
+
+#     if len(vrts) == 1:
+#         vrts = vrts[0]
+#     else:
+#         vrts = xr.concat(vrts, dim="band")
+    
+#     # open VRT
+#     # with xr.set_options(keep_attrs=True):
+#     # vrts = rxr.open_rasterio(URL[0])
+
+#     # index number and name of index for subsetting bands
+#     # var_idx = vrts.attrs['long_name'].index(varname.item()) 
+#     # var_key = [i for i in vrts.attrs['long_name'] if i == varname.item()]
+
+#     # if varname is Not none
+#     if varname is not None:
+        
+#         # vrts = vrts.isel(band=vrts.attrs['long_name'].index(varname.item()))
+#         if "long_name" in vrts.attrs.keys():
+
+#             if verbose:
+#                 print("Selecting varnames")
+#             vrts = vrts.sel(band = vrts.attrs['long_name'].index(varname.tolist()[0]))
+
+#     # subset by index if non "date" dimension
+#     if start is not None and end is None:
+#         vrts = vrts.isel(band=start)
+#     elif start is not None and end is not None:
+#         vrts = vrts.isel(band=slice(start, end))
+
+#     if grid is not None:
+#         xmin = grid.extent[0]
+#         ymin = grid.extent[1]
+#         xmax = grid.extent[2]
+#         ymax = grid.extent[3]
+
+#         # clip vrts to grid extent
+#         vrts = vrts.rio.clip_box(xmin, ymin, xmax, ymax)
+        
+#         # reproject vrts to grid CRS
+#         vrts.rio.write_crs(grid.crs, inplace=True)
+
+#         # flag as True if grid is given
+#         flag = True
+#     else:
+#         if (vrts.rio.crs.to_string() is None or vrts.rio.crs.to_string() == "") or all([i in [0, 1, 0, 1] for i in vrts.rio.bounds()]):
+#             if verbose:
+#                 print("Defined URL(s) are aspatial and on a unit grid. Cannot be cropped")
+
+#             # flag as False if missing CRS or if bounding box is [0, 1, 0, 1]
+#             flag = False
+#         else:
+#             # flag as True if no grid is given and nothing noteworthy
+#             flag = True
+
+#     # if an AOI is given and no flagging happens, crop and mask rasters to AOI
+#     if AOI is not None and flag:
+
+#         # Reproject the geometry to the CRS of the DataArray
+#         AOIv = AOI.to_crs(vrts.rio.crs)
+    
+#         # reproject AOI to vrts CRS
+#         # AOIv = AOI.to_crs(vrts.rio.crs, inplace=False).geometry.apply(lambda x: (x, 1))
+
+#         if verbose:
+#             print("Cropping/Clipping to AOI")
+#         # vrts.rio.
+#         # Crop the raster to the extent of the AOI
+#         # Crop and mask the DataArray to the polygon
+#         vrts = vrts.rio.clip(AOIv.geometry.apply(mapping))
+
+#         # dim that is NOT x or y
+#         selected_dim = [dim for dim in vrts.dims if dim not in ['x', 'y']][0]
+
+#         if "long_name" in vrts.attrs.keys():
+#             # delete extra long_name attributes
+#             del vrts.attrs['long_name']
+    
+#     # if toptobottom is True, flip the data vertically
+#     if toptobottom:
+        
+#         # print("Flipping data toptobottom")
+#         if verbose:
+#             print("Flipping data vertically")
+
+#         # vertically flip each 2D array
+#         flipped_data = np.flip(vrts.values, axis=0)
+
+#         # create new xarray DataArray from flipped NumPy array
+#         vrts = xr.DataArray(
+#             flipped_data,
+#             dims   = ('band', 'y', 'x'),
+#             coords = {'band': vrts[selected_dim], 'y': vrts.y, 'x': vrts.x}
+#             # dims   = ('y', 'x', 'time'),
+#             # coords = {'y': vrts_crop.y, 'x': vrts_crop.x, 'time': vrts_crop.time}
+#             )
+#     # vrts.close()
+
 #     return vrts
```

### Comparing `climatePy-0.0.4.1/climatePy/_shortcuts.py` & `climatePy-0.0.4.23/climatePy/_shortcuts.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1065 +1,1065 @@
-# Data manipulation tools
-import pandas as pd
-import geopandas as gpd
-import xarray as xr
-import shapely
-from shapely.geometry import Point
-# import matplotlib.pyplot as plt
-
-# import climatePy modules
-from . import _utils as utils
-from . import _dap as dap
-from . import _climatepy_filter as climatepy_filter
-
-# warnings lib
-import warnings
-
-# suppress warnings
-warnings.filterwarnings('ignore', category=Warning)
-
-# from src.climatePy import dap, climatepy_filter, utils
-# from climatePy import _utils, dap, climatepy_filter
-# from . import dap, climatepy_filter, utils
-# import ._utils as utils
-# import ._dap as dap
-# import ._climatepy_filter as climatepy_filter
-
-# test data
-# AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
-# AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
-
-# ----------------------
-# ---- getTerraClim ----
-# ----------------------
-
-def getTerraClim(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        verbose   = False
-        ):
-    
-    """Get Terra Climate Normals for an Area of Interest
-
-    These layers from TerraClimate were creating using climatically aided interpolation of monthly anomalies from the CRU Ts4.0 
-    and Japanese 55-year Reanalysis (JRA-55) datasets with WorldClim v2.0 climatologies.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to be extracted
-        startDate (str): Start date for data extraction in YYYY-MM-DD format
-        endDate (str): End date for data extraction in YYYY-MM-DD format
-        verbose (bool): Print out additional information
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-    # dap_meta = climatepy_dap(
-        AOI       = AOI, 
-        id        = "terraclim", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-    # dap_data = dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -----------------------------
-# ---- getTerraClimNormals ----
-# -----------------------------
-
-def getTerraClimNormals(
-        AOI       = None,
-        varname   = None,
-        month     = [i for i in range(1, 13)],
-        scenario  = '19812010', 
-        verbose   = False
-        ):
-    
-    """Get Terra Climate Normals for an Area of Interest
-
-    These layers from TerraClimate were creating using climatically aided interpolation of monthly anomalies 
-    from the CRU Ts4.0 and Japanese 55-year Reanalysis (JRA-55) datasets with WorldClim v2.0 climatologies.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to be extracted
-        month (int, list): Month(s) to extract data for
-        scenario (str): Scenario to extract data for
-        verbose (bool): Print out additional information
-    
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-
-    # make sure month is a list
-    if isinstance(month, int):
-        month = [month]
-
-    # collect raw meta data
-    raw = climatepy_filter.climatepy_filter(
-        # params    = params(), 
-        id        = "terraclim_normals", 
-        AOI       = AOI, 
-        varname   = varname, 
-        scenario  = scenario
-        )
-
-    # collect varname in correct order
-    varname = raw.varname.unique().tolist()
-
-    # collect duration string
-    durs = raw['duration'].iloc[0].split("/")
-    
-    # start and end dates for dap call
-    start_date = durs[0]
-    end_date   = durs[1]
-
-    # convert to datetime objects and create date range
-    dates = pd.date_range(start=start_date, end=end_date, freq='MS').tolist()
-
-    # select dates that match month input
-    dates = [i for i in dates if i.month in month]
-
-    # call dap
-    dap_data = dap.dap(
-        catalog   = raw, 
-        AOI       = AOI, 
-        startDate = min(dates).strftime("%Y-%m-%d"),
-        endDate   = max(dates).strftime("%Y-%m-%d"), 
-        varname   = varname,
-        verbose   = verbose
-        )
-
-    return dap_data
-
-# --------------------
-# ---- getGridMET ----
-# --------------------
-
-def getGridMET(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        verbose   = False
-        ):
-    
-    """Get GridMet Climate Data for an Area of Interest
-
-    gridMET is a dataset of daily high-spatial resolution (~4-km, 1/24th degree) surface meteorological data 
-    covering the contiguous US from 1979-yesterday. These data are updated daily.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (list): Variable name(s) to download. Options include:
-            ['pr', 'rmin', 'rmax', 'srad', 'sph', 'swe', 'tmmn', 'tmmx', 'vs', 'vpd', 'ws']
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        verbose (bool): Print verbose output
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "gridmet", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-    
-    # dap_meta['dopar'] = dopar
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# --------------------
-# ---- getGLDAS  ----
-# --------------------
-
-# TODO: ADD GLDAS and need check_rc_files() function 
-# def getGLDAS(
-#         AOI       = None,
-#         varname   = None,
-#         startDate = None, 
-#         endDate   = None, 
-#         model     = None,
-#         verbose   = False
-#         ):
-    
-#     """Get GLDAS Data for an Area of Interest
-
-#     Args:
-#         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-#         varname (list): Variable name(s) to download.
-#         startDate (str): Start date in the form "YYYY-MM-DD"
-#         endDate (str): End date in the form "YYYY-MM-DD"
-#         model (str): Model to download.
-#         verbose (bool): Print verbose output
-
-#     Returns:
-#         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-#     """
-
-#     # get matching arguments for climatepy_filter function
-#     dap_meta = dap.climatepy_dap(
-#         AOI       = AOI, 
-#         id        = "GLDAS", 
-#         varname   = varname, 
-#         startDate = startDate, 
-#         endDate   = endDate,
-#         verbose   = verbose
-#         )
-    
-#     # dap_meta['dopar'] = dopar
-
-#     # need to provide dap_meta dictionary object directly as input
-#     dap_data = dap.dap(
-#         **dap_meta
-#         )
-    
-#     return dap_data
-
-# -------------------
-# ---- getDaymet ----
-# -------------------
-
-def getDaymet(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        verbose   = False
-        ):
-    
-    """Get Daymet Climate Data for an Area of Interest
-
-    This dataset provides Daymet Version 4 model output data as gridded estimates of daily weather parameters for North America.
-    Daymet output variables include the following parameters: minimum temperature, maximum temperature, precipitation, shortwave radiation,
-    vapor pressure, snow water equivalent, and day length. The dataset covers the period from January 1, 1980 to December 31 of 
-    the most recent full calendar year. Each subsequent year is processed individually at the close of a calendar year after
-    allowing adequate time for input weather station data to be of archive quality.  Daymet variables are continuous surfaces provided as individual files,
-    by year, at a 1-km x 1-km spatial resolution and a daily temporal resolution. Data are in a Lambert Conformal
-    Conic projection for North America and are in a netCDF file format compliant with Climate and Forecast (CF) metadata conventions.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (list): Variable name(s) to download. Options include:	
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        verbose (bool): Print verbose output
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "daymet4", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -----------------
-# ---- getBCCA ----
-# -----------------
-
-def getBCCA(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None,
-        model     = 'CCSM4',
-        scenario  = 'rcp45', 
-        ensemble  = None,  
-        verbose   = False
-        ):
-    
-    """Get BCCA data for an Area of Interest
-
-    This dataset provides BCCA model output data as gridded estimates of daily weather parameters for North America.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download. Options include:
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        model (str): Model name. Default is 'CCSM4'.
-        scenario (str): Scenario name. Default is 'rcp45'.
-        ensemble (str): Ensemble name. Default is None.
-        verbose (bool): Print verbose output
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "bcca", 
-        varname   = varname, 
-        model     = model,
-        scenario  = scenario, 
-        ensemble  = ensemble, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# ------------------
-# ---- getPRISM ----
-# ------------------
-def getPRISM(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        timeRes   = None,
-        verbose   = False
-        ):
-    
-    """Get PRISM data for an Area of Interest
-        Currently only monthly data is available.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        timeRes (str): time resolution of data to be downloaded. Options are "daily" or "monthly". Default is "monthly"
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-
-    # TODO: setup timeRes argument so daily or monthly data can be got 
-    # # # check timeRes argument
-    if timeRes not in ['daily', 'monthly']:
-        raise ValueError("timeRes must be monthly or daily")
-
-    if timeRes is None:
-        # set timeRes argument
-        timeRes = "monthly"
-
-    if timeRes == "monthly":
-        # get matching arguments for climatepy_filter function
-        dap_meta = dap.climatepy_dap(
-            AOI       = AOI, 
-            id        = "prism_monthly",
-            # id        = "prism_" + timeRes, 
-            varname   = varname, 
-            startDate = startDate, 
-            endDate   = endDate,
-            verbose   = verbose
-            )
-
-        # need to provide dap_meta dictionary object directly as input
-        dap_data = dap.dap(
-            **dap_meta
-            )
-        
-        return dap_data
-    
-    elif timeRes == "daily":
-        dap_data = dap.get_prism_daily(
-            AOI       = AOI,
-            varname   = varname,
-            startDate = startDate,
-            endDate   = endDate,
-            verbose   = verbose
-            )
-        
-        return dap_data
-    
-    return dap_data
-
-# --------------------
-# ---- getLivneh ----
-# --------------------
-
-def getLivneh(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        timeRes   = "daily",
-        verbose   = False
-        ):
-    
-    """Get Livneh Climate Data for an Area of Interest
-
-    This dataset provides Livneh model output data as gridded estimates of daily weather parameters for North America.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        timeRes (str): Time resolution. Options include: "daily" or "monthly". Default is "daily".
-        verbose (bool): Print verbose output
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """
-
-    if timeRes == "daily":
-        # get matching arguments for climatepy_filter function
-        dap_meta = dap.climatepy_dap(
-            AOI       = AOI, 
-            id        = "Livneh_daily", 
-            varname   = varname, 
-            startDate = startDate, 
-            endDate   = endDate,
-            verbose   = verbose
-            )
-    else: 
-        # get matching arguments for climatepy_filter function
-        dap_meta = dap.climatepy_dap(
-            AOI       = AOI,
-            id        = "Livneh_monthly", 
-            varname   = varname, 
-            startDate = startDate, 
-            endDate   = endDate,
-            verbose   = verbose
-            )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# --------------------------
-# ---- getLivneh_fluxes ----
-# --------------------------
-
-def getLivneh_fluxes(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        verbose   = False
-        ):
-    
-    """Get Livneh Fluxes Climate Data for an Area of Interest
-
-    This dataset provides Livneh model output data as gridded estimates of daily weather parameters for North America.
-    
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        verbose (bool): Print verbose output
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """
-    
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "Livneh_fluxes", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# ----------------
-# ---- getVIC ----
-# ----------------
-
-def getVIC(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        model     = 'ccsm4', 
-        scenario  = 'rcp45',
-        verbose   = False
-        ):
-    
-    """Get VIC Climate Data for an Area of Interest"""
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "bcsd_vic", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        model     = model,
-        scenario  = scenario,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# ------------------
-# ---- getNLDAS ----
-# ------------------
-
-def getNLDAS(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        model     = None, 
-        verbose   = False
-        ):
-    
-    """Get NLDAS Climate Data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        model (str): Model name. Default is None.
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "NLDAS", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        model     = model,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -----------------
-# ---- getMACA ---- 
-# -----------------
-
-def getMACA(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        timeRes   = 'day',
-        model     = 'CCSM4', 
-        scenario  = 'rcp45', 
-        verbose   = False
-        ):
-    
-    """Get MACA Climate Data for an Area of Interest
-
-    Multivariate Adaptive Constructed Analogs (MACA) is a statistical method for downscaling Global Climate Models
-    (GCMs) from their native coarse resolution to a higher spatial resolution that captures reflects 
-    observed patterns of daily near-surface meteorology and simulated changes in GCMs experiments.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        timeRes (str): Time resolution. Either "mmonth" or "day". Default is 'day'.
-        model (str): Model name. Default is 'CCSM4'.
-        scenario (str): Scenario name. Default is 'rcp45'.
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-    
-    # check timeRes argument
-    if timeRes not in ['day', 'month']:
-        raise ValueError("timeRes must be month or day")
-    
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "maca_" + timeRes, 
-        varname   = varname, 
-        model     = model,
-        scenario  = scenario, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -------------------
-# ---- getCHIRPS ----
-# -------------------
-
-# TODO: too much data is extracted when function is called, need to look into what is going on here with the dap function
-# TODO: currently crashes my computer, even when I try to run on a small AOI and for a short time period
-def getCHIRPS(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        verbose   = False
-        ):
-    
-    """Get CHIRPS data for an Area of Interest
-
-    CHIRPS is a global dataset of daily precipitation estimates, with a spatial resolution of 0.05 degrees (~5 km).
-    Currently only monthly data is available.
-
-    Args:
-        AOI (geopandas dataframe, shapely geometry): Area of Interest polygon to extract data for.
-        varname (str): variable name to extract (e.g. tmin).
-        startDate (str): start date of data to be downloaded (YYYY-MM-DD). Default is None.
-        endDate (str): end date of data to be downloaded (YYYY-MM-DD). Default is None.
-        verbose (bool): print verbose output. Default is False.
-    """
-
-    timeRes = "monthly"
-
-    # make sure timeRes is capitalized correctly
-    timeRes = " ".join(word.capitalize() for word in timeRes.split())
-
-    # Regex to capitalize first letter of each word
-    # timeRes = re.sub(r"(^|[[:space:]])([[:alpha:]])",
-    # 	lambda match: match.group(1) + match.group(2).upper(), timeRes)
-
-    # correctly formatted timeRes values
-    good_timeRes = ["Pentad", "Annual", "Daily", "Monthly"]
-
-    # check timeRes argument is valid
-    if timeRes not in good_timeRes:
-        raise ValueError(f"timeRes must be one of: {', '.join(good_timeRes)}")
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "chirps20Global" + timeRes + "P05", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -----------------
-# ---- getLOCA ----
-# -----------------
-
-def getLOCA(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        model     = 'CCSM4',
-        scenario  = 'rcp45',
-        verbose   = False
-        ):
-    
-    """Get LOCA Climate Data for an Area of Interest
-
-    LOCA is a statistical downscaling technique that uses past history to add improved fine-scale detail to global climate models.
-
-    LOCA has been used to downscale 32 global climate models from the CMIP5 archive at a 1/16th degree spatial resolution, 
-    covering North America from central Mexico through Southern Canada. The historical period is 1950-2005,
-    and there are two future scenarios available: RCP 4.5 and RCP 8.5 over the period 2006-2100 (although some models stop in 2099). 
-    The variables currently available are daily minimum and maximum temperature, and daily precipitation.
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        model (str): Model name. Default is 'CCSM4'.
-        scenario (str): Scenario name. Default is 'rcp45'.
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "loca", 
-        varname   = varname, 
-        startDate = startDate, 
-        endDate   = endDate,
-        model     = model,
-        scenario  = scenario,
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# --------------------
-# ---- getPolaris ----
-# --------------------
-
-def getPolaris(
-        AOI       = None,
-        varname   = None,
-        verbose   = False
-        ):
-    
-    """Get Polaris Climate Data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-
-    """
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI, 
-        id        = "polaris", 
-        varname   = varname, 
-        verbose   = verbose
-        )
-
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# ---------------------
-# ---- getWordClim ----
-# ---------------------
-
-# TODO this function throws an error on the first call and succeeds on the second call (temp file issue?) 
-def getWorldClim(
-        AOI       = None,
-        varname   = None,
-        date 	  = None,
-        res       = None,
-        verbose   = False
-        ):
-    
-    """Get WorldClim data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        date (str): date in the form "YYYY-MM-DD"
-        res (str): Resolution of data to download. One of: "10m", "5m", "2.5m", "30s". Default is "10m".
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """	
-
-    if res is None:
-        res = "10m"
-    
-    if res not in ["10m", "5m", "2.5m", "30s"]:
-        raise ValueError("res must be one of: 10m, 5m, 2.5m, 30s")
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "wc2.1_" + res,
-        varname   = varname,
-        startDate = date,
-        endDate   = date,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# ------------------------
-# ---- getISRIC_soils ----
-# ------------------------
-# getSoilGrids vs getISRIC_soils
-
-def getISRIC_soils(
-        AOI       = None,
-        varname   = None,
-        date 	  = None,
-        res       = None,
-        verbose   = False
-        ):
-    
-    """Get ISRIC Soil Grids data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """	
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "ISRIC Soil Grids",
-        varname   = varname,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -----------------
-# ---- get3DEP ----
-# -----------------
-
-def get3DEP(
-        AOI       = None,
-        res       = None,
-        verbose   = False
-        ):
-    
-    """Get USGS Digatal Elevation Model (DEM) data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        res (str): Resolution of data to download. One of: "10m", "30m". Default is "30m".
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """	
-
-    if res is None:
-        res = '30m'
-
-    # check res argument
-    if res not in ['10m', '30m']:
-        raise ValueError("timeRes must be '10m' or '30m'")
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "USGS 3DEP",
-        asset     = res + " CONUS DEM",
-        varname   = "elevation",
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# --------------------
-# ---- getNASADEM ----
-# --------------------
-
-def getNASADEM(
-        AOI       = None,
-        verbose   = False
-        ):
-    
-    """Get NASA Digatal Elevation Model (DEM) data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """	
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "NASADEM",
-        varname   = "elevation",
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-# -------------------------
-# ---- AquaGoesSSTAnom ----
-# -------------------------
-
-def AquaGoesSSTAnom(
-        AOI       = None,
-        varname   = None,
-        startDate = None,
-        endDate   = None,
-        units     = None,
-        verbose   = False
-        ):
-    
-    """Get SST anomolies from AquaGoesSSTAnomC data for an Area of Interest
-
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in "YYYY-MM-DD" format.
-        endDate (str): End date in "YYYY-MM-DD" format.
-        units: temperature units to return data in "C" or "F". Default is "C".
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """	
-
-    if units == None:
-        units = "C"
-    
-    if units not in ["C", "F"]:
-        raise ValueError("units must be either 'C' or 'F'")
-    
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "aquaGoesSSTAnom" + units,
-        varname   = varname,
-        startDate = startDate,
-        endDate   = endDate,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
-
-
-# ------------------
-# ---- getLCMAP ----
-# ------------------
-
-def getLCMAP(
-        AOI       = None,
-        varname   = None,
-        startDate = None, 
-        endDate   = None, 
-        verbose   = False
-        ):
-    
-    """Get LCMAP data for an Area of Interest
-    
-    Args:
-        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
-        varname (str, list): Variable name(s) to download.
-        startDate (str): Start date in the form "YYYY-MM-DD"
-        endDate (str): End date in the form "YYYY-MM-DD"
-        verbose (bool): Print verbose output. Default is False.
-
-    Returns:
-        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
-    """	
-
-    # get matching arguments for climatepy_filter function
-    dap_meta = dap.climatepy_dap(
-        AOI       = AOI,
-        id        = "LCMAP",
-        varname   = varname,
-        startDate = startDate,
-        endDate   = endDate,
-        verbose   = verbose
-        )
-    
-    # need to provide dap_meta dictionary object directly as input
-    dap_data = dap.dap(
-        **dap_meta
-        )
-    
-    return dap_data
+# Data manipulation tools
+import pandas as pd
+import geopandas as gpd
+import xarray as xr
+import shapely
+from shapely.geometry import Point
+# import matplotlib.pyplot as plt
+
+# import climatePy modules
+from . import _utils as utils
+from . import _dap as dap
+from . import _climatepy_filter as climatepy_filter
+
+# warnings lib
+import warnings
+
+# suppress warnings
+warnings.filterwarnings('ignore', category=Warning)
+
+# from src.climatePy import dap, climatepy_filter, utils
+# from climatePy import _utils, dap, climatepy_filter
+# from . import dap, climatepy_filter, utils
+# import ._utils as utils
+# import ._dap as dap
+# import ._climatepy_filter as climatepy_filter
+
+# test data
+# AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
+# AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
+
+# ----------------------
+# ---- getTerraClim ----
+# ----------------------
+
+def getTerraClim(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        verbose   = False
+        ):
+    
+    """Get Terra Climate Normals for an Area of Interest
+
+    These layers from TerraClimate were creating using climatically aided interpolation of monthly anomalies from the CRU Ts4.0 
+    and Japanese 55-year Reanalysis (JRA-55) datasets with WorldClim v2.0 climatologies.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to be extracted
+        startDate (str): Start date for data extraction in YYYY-MM-DD format
+        endDate (str): End date for data extraction in YYYY-MM-DD format
+        verbose (bool): Print out additional information
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+    # dap_meta = climatepy_dap(
+        AOI       = AOI, 
+        id        = "terraclim", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+    # dap_data = dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -----------------------------
+# ---- getTerraClimNormals ----
+# -----------------------------
+
+def getTerraClimNormals(
+        AOI       = None,
+        varname   = None,
+        month     = [i for i in range(1, 13)],
+        scenario  = '19812010', 
+        verbose   = False
+        ):
+    
+    """Get Terra Climate Normals for an Area of Interest
+
+    These layers from TerraClimate were creating using climatically aided interpolation of monthly anomalies 
+    from the CRU Ts4.0 and Japanese 55-year Reanalysis (JRA-55) datasets with WorldClim v2.0 climatologies.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to be extracted
+        month (int, list): Month(s) to extract data for
+        scenario (str): Scenario to extract data for
+        verbose (bool): Print out additional information
+    
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+
+    # make sure month is a list
+    if isinstance(month, int):
+        month = [month]
+
+    # collect raw meta data
+    raw = climatepy_filter.climatepy_filter(
+        # params    = params(), 
+        id        = "terraclim_normals", 
+        AOI       = AOI, 
+        varname   = varname, 
+        scenario  = scenario
+        )
+
+    # collect varname in correct order
+    varname = raw.varname.unique().tolist()
+
+    # collect duration string
+    durs = raw['duration'].iloc[0].split("/")
+    
+    # start and end dates for dap call
+    start_date = durs[0]
+    end_date   = durs[1]
+
+    # convert to datetime objects and create date range
+    dates = pd.date_range(start=start_date, end=end_date, freq='MS').tolist()
+
+    # select dates that match month input
+    dates = [i for i in dates if i.month in month]
+
+    # call dap
+    dap_data = dap.dap(
+        catalog   = raw, 
+        AOI       = AOI, 
+        startDate = min(dates).strftime("%Y-%m-%d"),
+        endDate   = max(dates).strftime("%Y-%m-%d"), 
+        varname   = varname,
+        verbose   = verbose
+        )
+
+    return dap_data
+
+# --------------------
+# ---- getGridMET ----
+# --------------------
+
+def getGridMET(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        verbose   = False
+        ):
+    
+    """Get GridMet Climate Data for an Area of Interest
+
+    gridMET is a dataset of daily high-spatial resolution (~4-km, 1/24th degree) surface meteorological data 
+    covering the contiguous US from 1979-yesterday. These data are updated daily.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (list): Variable name(s) to download. Options include:
+            ['pr', 'rmin', 'rmax', 'srad', 'sph', 'swe', 'tmmn', 'tmmx', 'vs', 'vpd', 'ws']
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "gridmet", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+    
+    # dap_meta['dopar'] = dopar
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# --------------------
+# ---- getGLDAS  ----
+# --------------------
+
+# TODO: ADD GLDAS and need check_rc_files() function 
+# def getGLDAS(
+#         AOI       = None,
+#         varname   = None,
+#         startDate = None, 
+#         endDate   = None, 
+#         model     = None,
+#         verbose   = False
+#         ):
+    
+#     """Get GLDAS Data for an Area of Interest
+
+#     Args:
+#         AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+#         varname (list): Variable name(s) to download.
+#         startDate (str): Start date in the form "YYYY-MM-DD"
+#         endDate (str): End date in the form "YYYY-MM-DD"
+#         model (str): Model to download.
+#         verbose (bool): Print verbose output
+
+#     Returns:
+#         dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+#     """
+
+#     # get matching arguments for climatepy_filter function
+#     dap_meta = dap.climatepy_dap(
+#         AOI       = AOI, 
+#         id        = "GLDAS", 
+#         varname   = varname, 
+#         startDate = startDate, 
+#         endDate   = endDate,
+#         verbose   = verbose
+#         )
+    
+#     # dap_meta['dopar'] = dopar
+
+#     # need to provide dap_meta dictionary object directly as input
+#     dap_data = dap.dap(
+#         **dap_meta
+#         )
+    
+#     return dap_data
+
+# -------------------
+# ---- getDaymet ----
+# -------------------
+
+def getDaymet(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        verbose   = False
+        ):
+    
+    """Get Daymet Climate Data for an Area of Interest
+
+    This dataset provides Daymet Version 4 model output data as gridded estimates of daily weather parameters for North America.
+    Daymet output variables include the following parameters: minimum temperature, maximum temperature, precipitation, shortwave radiation,
+    vapor pressure, snow water equivalent, and day length. The dataset covers the period from January 1, 1980 to December 31 of 
+    the most recent full calendar year. Each subsequent year is processed individually at the close of a calendar year after
+    allowing adequate time for input weather station data to be of archive quality.  Daymet variables are continuous surfaces provided as individual files,
+    by year, at a 1-km x 1-km spatial resolution and a daily temporal resolution. Data are in a Lambert Conformal
+    Conic projection for North America and are in a netCDF file format compliant with Climate and Forecast (CF) metadata conventions.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (list): Variable name(s) to download. Options include:	
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "daymet4", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -----------------
+# ---- getBCCA ----
+# -----------------
+
+def getBCCA(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None,
+        model     = 'CCSM4',
+        scenario  = 'rcp45', 
+        ensemble  = None,  
+        verbose   = False
+        ):
+    
+    """Get BCCA data for an Area of Interest
+
+    This dataset provides BCCA model output data as gridded estimates of daily weather parameters for North America.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download. Options include:
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        model (str): Model name. Default is 'CCSM4'.
+        scenario (str): Scenario name. Default is 'rcp45'.
+        ensemble (str): Ensemble name. Default is None.
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "bcca", 
+        varname   = varname, 
+        model     = model,
+        scenario  = scenario, 
+        ensemble  = ensemble, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# ------------------
+# ---- getPRISM ----
+# ------------------
+def getPRISM(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        timeRes   = None,
+        verbose   = False
+        ):
+    
+    """Get PRISM data for an Area of Interest
+        Currently only monthly data is available.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        timeRes (str): time resolution of data to be downloaded. Options are "daily" or "monthly". Default is "monthly"
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+
+    # TODO: setup timeRes argument so daily or monthly data can be got 
+    # # # check timeRes argument
+    if timeRes not in ['daily', 'monthly']:
+        raise ValueError("timeRes must be monthly or daily")
+
+    if timeRes is None:
+        # set timeRes argument
+        timeRes = "monthly"
+
+    if timeRes == "monthly":
+        # get matching arguments for climatepy_filter function
+        dap_meta = dap.climatepy_dap(
+            AOI       = AOI, 
+            id        = "prism_monthly",
+            # id        = "prism_" + timeRes, 
+            varname   = varname, 
+            startDate = startDate, 
+            endDate   = endDate,
+            verbose   = verbose
+            )
+
+        # need to provide dap_meta dictionary object directly as input
+        dap_data = dap.dap(
+            **dap_meta
+            )
+        
+        return dap_data
+    
+    elif timeRes == "daily":
+        dap_data = dap.get_prism_daily(
+            AOI       = AOI,
+            varname   = varname,
+            startDate = startDate,
+            endDate   = endDate,
+            verbose   = verbose
+            )
+        
+        return dap_data
+    
+    return dap_data
+
+# --------------------
+# ---- getLivneh ----
+# --------------------
+
+def getLivneh(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        timeRes   = "daily",
+        verbose   = False
+        ):
+    
+    """Get Livneh Climate Data for an Area of Interest
+
+    This dataset provides Livneh model output data as gridded estimates of daily weather parameters for North America.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        timeRes (str): Time resolution. Options include: "daily" or "monthly". Default is "daily".
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+
+    if timeRes == "daily":
+        # get matching arguments for climatepy_filter function
+        dap_meta = dap.climatepy_dap(
+            AOI       = AOI, 
+            id        = "Livneh_daily", 
+            varname   = varname, 
+            startDate = startDate, 
+            endDate   = endDate,
+            verbose   = verbose
+            )
+    else: 
+        # get matching arguments for climatepy_filter function
+        dap_meta = dap.climatepy_dap(
+            AOI       = AOI,
+            id        = "Livneh_monthly", 
+            varname   = varname, 
+            startDate = startDate, 
+            endDate   = endDate,
+            verbose   = verbose
+            )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# --------------------------
+# ---- getLivneh_fluxes ----
+# --------------------------
+
+def getLivneh_fluxes(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        verbose   = False
+        ):
+    
+    """Get Livneh Fluxes Climate Data for an Area of Interest
+
+    This dataset provides Livneh model output data as gridded estimates of daily weather parameters for North America.
+    
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        verbose (bool): Print verbose output
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+    
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "Livneh_fluxes", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# ----------------
+# ---- getVIC ----
+# ----------------
+
+def getVIC(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        model     = 'ccsm4', 
+        scenario  = 'rcp45',
+        verbose   = False
+        ):
+    
+    """Get VIC Climate Data for an Area of Interest"""
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "bcsd_vic", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        model     = model,
+        scenario  = scenario,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# ------------------
+# ---- getNLDAS ----
+# ------------------
+
+def getNLDAS(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        model     = None, 
+        verbose   = False
+        ):
+    
+    """Get NLDAS Climate Data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        model (str): Model name. Default is None.
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "NLDAS", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        model     = model,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -----------------
+# ---- getMACA ---- 
+# -----------------
+
+def getMACA(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        timeRes   = 'day',
+        model     = 'CCSM4', 
+        scenario  = 'rcp45', 
+        verbose   = False
+        ):
+    
+    """Get MACA Climate Data for an Area of Interest
+
+    Multivariate Adaptive Constructed Analogs (MACA) is a statistical method for downscaling Global Climate Models
+    (GCMs) from their native coarse resolution to a higher spatial resolution that captures reflects 
+    observed patterns of daily near-surface meteorology and simulated changes in GCMs experiments.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        timeRes (str): Time resolution. Either "mmonth" or "day". Default is 'day'.
+        model (str): Model name. Default is 'CCSM4'.
+        scenario (str): Scenario name. Default is 'rcp45'.
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+    
+    # check timeRes argument
+    if timeRes not in ['day', 'month']:
+        raise ValueError("timeRes must be month or day")
+    
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "maca_" + timeRes, 
+        varname   = varname, 
+        model     = model,
+        scenario  = scenario, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -------------------
+# ---- getCHIRPS ----
+# -------------------
+
+# TODO: too much data is extracted when function is called, need to look into what is going on here with the dap function
+# TODO: currently crashes my computer, even when I try to run on a small AOI and for a short time period
+def getCHIRPS(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        verbose   = False
+        ):
+    
+    """Get CHIRPS data for an Area of Interest
+
+    CHIRPS is a global dataset of daily precipitation estimates, with a spatial resolution of 0.05 degrees (~5 km).
+    Currently only monthly data is available.
+
+    Args:
+        AOI (geopandas dataframe, shapely geometry): Area of Interest polygon to extract data for.
+        varname (str): variable name to extract (e.g. tmin).
+        startDate (str): start date of data to be downloaded (YYYY-MM-DD). Default is None.
+        endDate (str): end date of data to be downloaded (YYYY-MM-DD). Default is None.
+        verbose (bool): print verbose output. Default is False.
+    """
+
+    timeRes = "monthly"
+
+    # make sure timeRes is capitalized correctly
+    timeRes = " ".join(word.capitalize() for word in timeRes.split())
+
+    # Regex to capitalize first letter of each word
+    # timeRes = re.sub(r"(^|[[:space:]])([[:alpha:]])",
+    # 	lambda match: match.group(1) + match.group(2).upper(), timeRes)
+
+    # correctly formatted timeRes values
+    good_timeRes = ["Pentad", "Annual", "Daily", "Monthly"]
+
+    # check timeRes argument is valid
+    if timeRes not in good_timeRes:
+        raise ValueError(f"timeRes must be one of: {', '.join(good_timeRes)}")
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "chirps20Global" + timeRes + "P05", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -----------------
+# ---- getLOCA ----
+# -----------------
+
+def getLOCA(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        model     = 'CCSM4',
+        scenario  = 'rcp45',
+        verbose   = False
+        ):
+    
+    """Get LOCA Climate Data for an Area of Interest
+
+    LOCA is a statistical downscaling technique that uses past history to add improved fine-scale detail to global climate models.
+
+    LOCA has been used to downscale 32 global climate models from the CMIP5 archive at a 1/16th degree spatial resolution, 
+    covering North America from central Mexico through Southern Canada. The historical period is 1950-2005,
+    and there are two future scenarios available: RCP 4.5 and RCP 8.5 over the period 2006-2100 (although some models stop in 2099). 
+    The variables currently available are daily minimum and maximum temperature, and daily precipitation.
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        model (str): Model name. Default is 'CCSM4'.
+        scenario (str): Scenario name. Default is 'rcp45'.
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "loca", 
+        varname   = varname, 
+        startDate = startDate, 
+        endDate   = endDate,
+        model     = model,
+        scenario  = scenario,
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# --------------------
+# ---- getPolaris ----
+# --------------------
+
+def getPolaris(
+        AOI       = None,
+        varname   = None,
+        verbose   = False
+        ):
+    
+    """Get Polaris Climate Data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+
+    """
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI, 
+        id        = "polaris", 
+        varname   = varname, 
+        verbose   = verbose
+        )
+
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# ---------------------
+# ---- getWordClim ----
+# ---------------------
+
+# TODO this function throws an error on the first call and succeeds on the second call (temp file issue?) 
+def getWorldClim(
+        AOI       = None,
+        varname   = None,
+        date 	  = None,
+        res       = None,
+        verbose   = False
+        ):
+    
+    """Get WorldClim data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        date (str): date in the form "YYYY-MM-DD"
+        res (str): Resolution of data to download. One of: "10m", "5m", "2.5m", "30s". Default is "10m".
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """	
+
+    if res is None:
+        res = "10m"
+    
+    if res not in ["10m", "5m", "2.5m", "30s"]:
+        raise ValueError("res must be one of: 10m, 5m, 2.5m, 30s")
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "wc2.1_" + res,
+        varname   = varname,
+        startDate = date,
+        endDate   = date,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# ------------------------
+# ---- getISRIC_soils ----
+# ------------------------
+# getSoilGrids vs getISRIC_soils
+
+def getISRIC_soils(
+        AOI       = None,
+        varname   = None,
+        date 	  = None,
+        res       = None,
+        verbose   = False
+        ):
+    
+    """Get ISRIC Soil Grids data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """	
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "ISRIC Soil Grids",
+        varname   = varname,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -----------------
+# ---- get3DEP ----
+# -----------------
+
+def get3DEP(
+        AOI       = None,
+        res       = None,
+        verbose   = False
+        ):
+    
+    """Get USGS Digatal Elevation Model (DEM) data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        res (str): Resolution of data to download. One of: "10m", "30m". Default is "30m".
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """	
+
+    if res is None:
+        res = '30m'
+
+    # check res argument
+    if res not in ['10m', '30m']:
+        raise ValueError("timeRes must be '10m' or '30m'")
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "USGS 3DEP",
+        asset     = res + " CONUS DEM",
+        varname   = "elevation",
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# --------------------
+# ---- getNASADEM ----
+# --------------------
+
+def getNASADEM(
+        AOI       = None,
+        verbose   = False
+        ):
+    
+    """Get NASA Digatal Elevation Model (DEM) data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """	
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "NASADEM",
+        varname   = "elevation",
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+# -------------------------
+# ---- AquaGoesSSTAnom ----
+# -------------------------
+
+def AquaGoesSSTAnom(
+        AOI       = None,
+        varname   = None,
+        startDate = None,
+        endDate   = None,
+        units     = None,
+        verbose   = False
+        ):
+    
+    """Get SST anomolies from AquaGoesSSTAnomC data for an Area of Interest
+
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in "YYYY-MM-DD" format.
+        endDate (str): End date in "YYYY-MM-DD" format.
+        units: temperature units to return data in "C" or "F". Default is "C".
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """	
+
+    if units == None:
+        units = "C"
+    
+    if units not in ["C", "F"]:
+        raise ValueError("units must be either 'C' or 'F'")
+    
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "aquaGoesSSTAnom" + units,
+        varname   = varname,
+        startDate = startDate,
+        endDate   = endDate,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
+
+
+# ------------------
+# ---- getLCMAP ----
+# ------------------
+
+def getLCMAP(
+        AOI       = None,
+        varname   = None,
+        startDate = None, 
+        endDate   = None, 
+        verbose   = False
+        ):
+    
+    """Get LCMAP data for an Area of Interest
+    
+    Args:
+        AOI (shapely.geometry.polygon.Polygon): Area of interest as a shapely polygon or geopandas dataframe
+        varname (str, list): Variable name(s) to download.
+        startDate (str): Start date in the form "YYYY-MM-DD"
+        endDate (str): End date in the form "YYYY-MM-DD"
+        verbose (bool): Print verbose output. Default is False.
+
+    Returns:
+        dictionary of xarray.DataArray(s): xarray DataArray containing climate data
+    """	
+
+    # get matching arguments for climatepy_filter function
+    dap_meta = dap.climatepy_dap(
+        AOI       = AOI,
+        id        = "LCMAP",
+        varname   = varname,
+        startDate = startDate,
+        endDate   = endDate,
+        verbose   = verbose
+        )
+    
+    # need to provide dap_meta dictionary object directly as input
+    dap_data = dap.dap(
+        **dap_meta
+        )
+    
+    return dap_data
```

### Comparing `climatePy-0.0.4.1/climatePy/data/catalog.csv` & `climatePy-0.0.4.23/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.0.4.1/climatePy.egg-info/PKG-INFO` & `climatePy-0.0.4.23/climatePy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,196 @@
-Metadata-Version: 2.1
-Name: climatePy
-Version: 0.0.4.1
-Summary: A Python package for getting point and gridded climate data by AOI
-Author: Angus Watters, Mike Johnson
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# [**climatePy**](https://github.com/LynkerIntel/climatePy)
-
-<!-- badges: start -->
-
-[![stage](https://img.shields.io/badge/stage-dev-orange)](#)
-[![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
-[![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
-
-<!-- badges: end -->
-
-## Description
-
-A Python ðŸ“¦ for getting point and gridded climate data by AOI. `climatePy` is the Python version of the [`climateR`](https://github.com/mikejohnson51/climateR) R package, providing all of the same functionality but in Python.
-
-As its stated in the [climateR README](https://github.com/mikejohnson51/climateR#climater):
-climatePy simplifies the steps needed to get climate data into Python. At its core it provides three main things:
-
-1. A climate catalog of over 100,000k datasets from over 2,000 data providers/archives. See (`params()`)
-
-2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
-
-3. A set of shortcuts that implement these methods for a core set of selected catalog elements
-
-<br>
-
----
-
-- [climatePy PyPI](https://pypi.org/project/climatePy/)
-- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
-
----
-
-## Table of Contents (Optional)
-
-- [Installation](#installation)
-- [Usage](#usage)
-- [Credits](#credits)
-- [License](#license)
-- [How to Contribute](#how-to-contribute)
-
-<br>
-
-## Installation
-
-`climatePy` can be downloaded from PyPI via `pip` like so:
-
-``` 
-pip install climatePy
-```
-**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
-
-<br>
-
-## Usage
-
-### Loading climate catalog
-
-```python
-import geopandas as gpd
-import matplotlib.pyplot as plt
-from climatePy import params
-
-# load climate catalog
-catalog = params()
-
-# load example AOI data
-AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
-```
-<br>
-
-### Using `climatepy_filter()`:
-
-The `climatepy_filter()` is one of the core functions of `climatePy` and is used to do the first round of filtering on the base climate catalog.
-
-Here we filter down our climate catalog to TerraClim precipitation data for San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-raw = climatePy.climatepy_filter(
-        id        = "terraclim", 
-        AOI       = AOI, 
-        varname   = "ppt"
-        )
-```
-
-| id  | asset | varname    |
-|-------|-----|---------|
-| gridmet | agg_terraclimate_ppt_1958_CurrentYear_GLOBE  | ppt   |
-
-### AOI
-![San Luis Obispo County county](assets/images/san_luis_obispo_county_polygon.png)
-
-<br>
-
-### Getting climate data in AOI
-
-Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-prcp = shortcuts.getTerraClim(
-    AOI       = AOI,
-    varname   = "ppt",
-    startDate = "2018-01-01",
-    endDate   = "2018-01-01"
-    )
-```
-![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
-
-<br>
-<br>
-
-### Get data within a date range
-
-We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
-
-```python
-# collect raw meta data
-prcp = shortcuts.getTerraClim(
-    AOI       = AOI,
-    varname   = "ppt",
-    startDate = "2018-01-01",
-    endDate   = "2018-12-01"
-    )
-```
-![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
-
-<br>
-<br>
-
-## Credits
-
-Credit to [Mike J Johnson](https://github.com/mikejohnson51) and the other contributors to the original [`climateR`](https://github.com/mikejohnson51/climateR) package listed below:
-- [Max Joseph](https://github.com/mbjoseph)
-- [Eric R. Scott](https://github.com/Aariq)
-- [James Tsakalos](https://github.com/jamestsakalos)
-
-<br>
-
-## License
-
-MIT License
-
-Copyright (c) 2023 Angus Watters, Mike J. Johnson
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
----
-
-<br>
-
-## How to Contribute
-If you would like to contribute, submit a PR and we will get to as soon as we can!
-If you have any issues please open an issue on GitHub. For any questions, feel free to ask [@anguswg-ucsb](https://github.com/anguswg-ucsb) or [@mikejohnson51](https://github.com/mikejohnson51), or simply create an issue on GitHub.
+Metadata-Version: 2.1
+Name: climatePy
+Version: 0.0.4.23
+Summary: A Python package for getting point and gridded climate data by AOI
+Author: Angus Watters, Mike Johnson
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# [**climatePy**](https://github.com/LynkerIntel/climatePy)
+
+<!-- badges: start -->
+
+[![stage](https://img.shields.io/badge/stage-dev-orange)](#)
+[![Dependencies](https://img.shields.io/badge/dependencies-04/12-orange?style=flat)](#)
+[![License:
+MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+
+<!-- badges: end -->
+
+## Description
+
+A Python 📦 for getting point and gridded climate data by AOI. `climatePy` is the Python version of the [`climateR`](https://github.com/mikejohnson51/climateR) R package, providing all of the same functionality but in Python.
+
+As its stated in the [climateR README](https://github.com/mikejohnson51/climateR#climater):
+climatePy simplifies the steps needed to get climate data into Python. At its core it provides three main things:
+
+1. A climate catalog of over 100,000k datasets from over 2,000 data providers/archives. See (`params()`)
+
+2. A general toolkit for accessing remote and local gridded data files bounded by space, time, and variable constraints (`dap()`, `dap_crop()`, `read_dap_file()`)
+
+3. A set of shortcuts that implement these methods for a core set of selected catalog elements
+
+<br>
+
+---
+
+- [climatePy PyPI](https://pypi.org/project/climatePy/)
+- A slideshow walking through the capabilities of [**climateR/climatePy**](https://mikejohnson51.github.io/climateR-intro/#1)
+
+---
+
+## Table of Contents (Optional)
+
+- [Installation](#installation)
+- [Usage](#usage)
+- [Credits](#credits)
+- [License](#license)
+- [How to Contribute](#how-to-contribute)
+
+<br>
+
+## Installation
+
+`climatePy` can be downloaded from PyPI via `pip` like so:
+
+``` 
+pip install climatePy
+```
+**Note:** climatePy is still in **development** so expect to run into issues at this point in its lifecycle...
+
+<br>
+
+## Usage
+
+### Loading climate catalog
+
+```python
+import geopandas as gpd
+import matplotlib.pyplot as plt
+from climatePy import params
+
+# load climate catalog
+catalog = params()
+
+# load example AOI data
+AOI = gpd.read_file('src/data/san_luis_obispo_county.gpkg')
+```
+<br>
+
+### Using `climatepy_filter()`:
+
+The `climatepy_filter()` is one of the core functions of `climatePy` and is used to do the first round of filtering on the base climate catalog.
+
+Here we filter down our climate catalog to TerraClim precipitation data for San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+raw = climatePy.climatepy_filter(
+        id        = "terraclim", 
+        AOI       = AOI, 
+        varname   = "ppt"
+        )
+```
+
+| id  | asset | varname    |
+|-------|-----|---------|
+| gridmet | agg_terraclimate_ppt_1958_CurrentYear_GLOBE  | ppt   |
+
+### AOI
+![San Luis Obispo County county](assets/images/san_luis_obispo_county_polygon.png)
+
+<br>
+
+### Getting climate data in AOI
+
+Now lets use the `getTerraClim()` function from `climatePy` to get precipitation data for January 1st, 2018 in San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+prcp = shortcuts.getTerraClim(
+    AOI       = AOI,
+    varname   = "ppt",
+    startDate = "2018-01-01",
+    endDate   = "2018-01-01"
+    )
+```
+![Precipitation San Luis Obispo County](assets/images/san_luis_obispo_county_ppt.png)
+
+<br>
+<br>
+
+### Get data within a date range
+
+We can also get data within a date range. we'll use `getTerraClim()` to get monthly precipitation data for all of 2018 in San Luis Obispo County, CA.
+
+```python
+# collect raw meta data
+prcp = shortcuts.getTerraClim(
+    AOI       = AOI,
+    varname   = "ppt",
+    startDate = "2018-01-01",
+    endDate   = "2018-12-01"
+    )
+```
+![2018 precipitation in San Luis Obispo County, CA](assets/images/slo_prcp_facet_plots.png)
+
+<br>
+
+### Data from known bounding coordinates
+
+`climatePy` offers support for `shapely` bounding boxes. Here we are requesting wind velocity data for the four corners region of the USA by bounding coordinates.
+
+```python
+from shapely.geometry import box
+
+bbox = box(-112, 34, -105, 39)
+
+bbox = gpd.GeoDataFrame(geometry=[bbox], crs ='EPSG:4326')
+
+vs = climatePy.getGridMET(
+       AOI       = bbox, 
+       varname   = "vs",
+       startDate = "2018-09-01"
+       )
+```
+![Daily Wind Velocity Four Corners, USA](assets/images/four_corners_gridmet.png)
+
+<br>
+<br>
+
+## Credits
+
+Credit to [Mike J Johnson](https://github.com/mikejohnson51) and the other contributors to the original [`climateR`](https://github.com/mikejohnson51/climateR) package listed below:
+- [Max Joseph](https://github.com/mbjoseph)
+- [Eric R. Scott](https://github.com/Aariq)
+- [James Tsakalos](https://github.com/jamestsakalos)
+
+<br>
+
+## License
+
+MIT License
+
+Copyright (c) 2023 Angus Watters, Mike J. Johnson
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+---
+
+<br>
+
+## How to Contribute
+If you would like to contribute, submit a PR and we will get to as soon as we can!
+If you have any issues please open an issue on GitHub. For any questions, feel free to ask [@anguswg-ucsb](https://github.com/anguswg-ucsb) or [@mikejohnson51](https://github.com/mikejohnson51), or simply create an issue on GitHub.
```

### Comparing `climatePy-0.0.4.1/setup.py` & `climatePy-0.0.4.23/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import setuptools
-# from setuptools import setup, find_packages
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="climatePy",                         # pkg name
-    version="0.0.4.1",                        # version
-    author="Angus Watters, Mike Johnson",     # authors
-    description="A Python package for getting point and gridded climate data by AOI",
-    long_description=long_description,      # long description is read from the the readme file
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),    # python modules to install
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],          
-    python_requires='>=3.6',               # min python version required 
-    # py_modules=["climatePy"],             #  python package name
-    # package_dir={'':'climatePy/src'},     #  source code directory of package
-    # package_dir={'':'src/climatePy'},     #  source code directory of package
-    # package_dir={'':'/climatePy'},     #  source code directory of package
-    install_requires=['pandas', 'geopandas', 'shapely', 'pyproj', 'rasterio', 'xarray', 'rtree', 'numpy',
-                    'netCDF4', 'joblib'], # dependencies
-    include_package_data=True, 
-    package_data={'': ['data/*.csv']}     # include catalog csv dataset
-    # package_data={'src/climatePy': ['src/data/*']}
-)
+import setuptools
+# from setuptools import setup, find_packages
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="climatePy",                         # pkg name
+    version="0.0.4.23",                        # version
+    author="Angus Watters, Mike Johnson",     # authors
+    description="A Python package for getting point and gridded climate data by AOI",
+    long_description=long_description,      # long description is read from the the readme file
+    long_description_content_type="text/markdown",
+    packages=setuptools.find_packages(),    # python modules to install
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],          
+    python_requires='>=3.6',               # min python version required 
+    # py_modules=["climatePy"],             #  python package name
+    # package_dir={'':'climatePy/src'},     #  source code directory of package
+    # package_dir={'':'src/climatePy'},     #  source code directory of package
+    # package_dir={'':'/climatePy'},     #  source code directory of package
+    install_requires=['pandas', 'geopandas', 'shapely', 'pyproj', 'rasterio', 'xarray', 'rtree', 'numpy',
+                    'netCDF4', 'joblib'], # dependencies
+    include_package_data=True, 
+    package_data={'': ['data/*.csv']}     # include catalog csv dataset
+    # package_data={'src/climatePy': ['src/data/*']}
+    )
```

### Comparing `climatePy-0.0.4.1/tests/test_shortcuts.py` & `climatePy-0.0.4.23/tests/test_shortcuts.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1104 +1,1104 @@
-# pytest library
-import pytest
-
-# import climatePy modules
-import climatePy
-
-# data manipulation libs
-import pandas as pd
-import geopandas as gpd
-import xarray as xr
-
-# standard python libs
-import re
-from datetime import datetime
-
-
-# old imports
-# from .climatePy import shortcuts
-# from src.climatePy import shortcuts
-# from src.climatePy import dap
-# from src.climatePy import climatepy_filter
-# from src.climatePy import utils
-
-# AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
-# AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
-
-# @pytest.fixture(params=['miami_dade_county', 'san_luis_obispo_county', 
-#                         'litchfield_county', 'tuscaloosa_county', 
-#                         'boulder_county', 'king_county'])
-
-@pytest.fixture(params=['san_luis_obispo_county', 'boulder_county'])
-
-def AOI(request): 
-    # filepath = f'src/data/{request.param}.gpkg'
-    filepath = f'climatePy/data/{request.param}.gpkg'
-    AOI = gpd.read_file(filepath)
-    yield AOI
-
-def test_getTerraClim_case1(AOI):
-
-    varname = ["ppt", "tmax"]
-    startDate = "2018-01-01"
-    endDate   = "2018-03-02"
-    verbose   = True
-
-    # Call function to get output
-    output = climatePy.getTerraClim( AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"ppt", "tmax"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["ppt"], xr.DataArray)
-    assert isinstance(output["tmax"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["ppt"].dims == ("y", "x", "time")
-    assert output["tmax"].dims == ("y", "x", "time")   
-
-    dates1 = [datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values]
-    dates2 = [datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values]
-    
-    start_date1 = min(dates1)
-    end_date1   = max(dates1)
-    start_date2 = min(dates2)
-    end_date2   = max(dates2)
-
-    assert end_date1 - start_date1 == pd.Timedelta("59D")
-    assert end_date2 - start_date2 == pd.Timedelta("59D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-
-    assert "ppt" in output["ppt"].time[0].values.item()
-    assert "tmax" in output["tmax"].time[0].values.item()
-
-def test_getGridMET_case1(AOI):
-    # ---- Case 1 ----
-    verbose   = True
-    varname = "pr"
-    startDate="2000-01-01"
-    endDate="2000-01-01"
-    
-    # Call function to get output
-    output = climatePy.getGridMET( AOI, varname, startDate, endDate, verbose)
-    
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"pr"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
-    
-    assert end_date1 - start_date1 == pd.Timedelta("0D")
-
-    assert "pr" in output["pr"].time[0].values.item()
-    assert len(output["pr"].time.values) == 1
-
-def test_getGridMET_case2(AOI):    
-    # ---- Case 2 ----
-    verbose   = True
-    varname = ["pr", "tmmx"]
-    startDate = "2018-01-01"
-    endDate   = "2018-01-02"
-
-    # Call function to get output
-    output = climatePy.getGridMET( AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"tmmx", "pr"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-    assert isinstance(output["tmmx"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-    assert output["tmmx"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
-    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
-    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
-    
-    assert end_date1 - start_date1 == pd.Timedelta("1D")
-    assert end_date2 - start_date2 == pd.Timedelta("1D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-
-    assert "pr" in output["pr"].time[0].values.item()
-    assert "tmmx" in output["tmmx"].time[0].values.item()
-    assert len(output["pr"].time.values) == 2
-    assert len(output["tmmx"].time.values) == 2
-
-def test_getGridMET_case3(AOI):
-    # ---- Case 3 ----
-    verbose = True
-    varname = ["pr", "tmmx", "rmin"]
-    startDate = "2015-01-01"
-    endDate   = "2016-02-05"
-
-    # Call function to get output
-    output = climatePy.getGridMET( AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"tmmx", "pr", "rmin"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-    assert isinstance(output["tmmx"], xr.DataArray)
-    assert isinstance(output["rmin"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-    assert output["tmmx"].dims == ("y", "x", "time")
-    assert output["rmin"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
-    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
-    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
-    start_date3 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
-    end_date3   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
-
-    assert end_date1 - start_date1 == pd.Timedelta("400D")
-    assert end_date2 - start_date2 == pd.Timedelta("400D")
-    assert end_date3 - start_date3 == pd.Timedelta("400D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-    assert end_date3 - end_date2 == pd.Timedelta("0D")
-
-    assert "pr" in output["pr"].time[0].values.item()
-    assert "tmmx" in output["tmmx"].time[0].values.item()
-    assert "rmin" in output["rmin"].time[0].values.item()
-
-    assert len(output["pr"].time.values) == 401
-    assert len(output["tmmx"].time.values) == 401
-    assert len(output["rmin"].time.values) == 401
-    
-def test_getGridMET_case4(AOI):
-    # ---- Case 4 ----
-    verbose = True
-    varname = ["rmin"]
-    startDate = "2005-01-01"
-    endDate   = "2010-01-01"
-
-    # Call function to get output
-    output = climatePy.getGridMET(AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"rmin"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["rmin"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["rmin"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
-
-    assert end_date1 - start_date1 == pd.Timedelta("1826D")
-
-    assert "rmin" in output["rmin"].time[0].values.item()
-    assert len(output["rmin"].time.values) == 1827
-
-    
-def test_getTerraClimNormals_case1(AOI):
-    
-    # ---- Case 1 ----
-    verbose   = True
-    varname = ["ppt", "tmax"]
-    scenario  = '19611990'
-    month     = [1, 2]
-
-    # call function
-    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"ppt", "tmax"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["ppt"], xr.DataArray)
-    assert isinstance(output["tmax"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["ppt"].dims == ("y", "x", "time")
-    assert output["tmax"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    
-    assert end_date1 - start_date1 == pd.Timedelta("31D")
-    assert end_date2 - start_date2 == pd.Timedelta("31D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-
-    # check time variables names are correct
-    assert "ppt" in output["ppt"].time[0].values.item()
-    assert "tmax" in output["tmax"].time[0].values.item()
-    assert scenario in output["ppt"].time[0].values.item()
-    assert scenario in output["tmax"].time[0].values.item()
-    assert len(output["ppt"].time.values) == 2
-    assert len(output["tmax"].time.values) == 2
-
-def test_getTerraClimNormals_case2(AOI):
-
-    # ---- Case 2 ----
-    verbose   = True
-    varname = ["ppt", "tmax"]
-    scenario  = '19812010'
-    month     = [i for i in range(1, 13)]
-
-    # call function
-    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"ppt", "tmax"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["ppt"], xr.DataArray)
-    assert isinstance(output["tmax"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["ppt"].dims == ("y", "x", "time")
-    assert output["tmax"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    
-    assert end_date1 - start_date1 == pd.Timedelta("334D")
-    assert end_date2 - start_date2 == pd.Timedelta("334D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-
-    # check time variables names are correct
-    assert "ppt" in output["ppt"].time[0].values.item()
-    assert "tmax" in output["tmax"].time[0].values.item()
-    assert scenario in output["ppt"].time[0].values.item()
-    assert scenario in output["tmax"].time[0].values.item()
-    assert len(output["ppt"].time.values) == 12
-    assert len(output["tmax"].time.values) == 12
-
-def test_getTerraClimNormals_case3(AOI):
-    # ---- Case 3 ----
-    verbose   = True
-    varname = ["ppt", "tmax"]
-    scenario = '2C'
-    month     = [1, 3]
-
-    # call function
-    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"ppt", "tmax"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["ppt"], xr.DataArray)
-    assert isinstance(output["tmax"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["ppt"].dims == ("y", "x", "time")
-    assert output["tmax"].dims == ("y", "x", "time")
-
-    # Assert dates are correct
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    
-    assert end_date1 - start_date1 == pd.Timedelta("59D")
-    assert end_date2 - start_date2 == pd.Timedelta("59D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-
-    # check time variables names are correct
-    assert "ppt" in output["ppt"].time[0].values.item()
-    assert "tmax" in output["tmax"].time[0].values.item()
-    assert scenario in output["ppt"].time[0].values.item()
-    assert scenario in output["tmax"].time[0].values.item()
-    assert len(output["ppt"].time.values) == 3
-    assert len(output["tmax"].time.values) == 3
-    
-def test_getTerraClimNormals_case4(AOI):
-    # ---- Case 4 ----
-    verbose   = True
-    varname = ["ppt", "tmax"]
-    scenario = '4C'
-    month     = [1]
-    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"ppt", "tmax"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["ppt"], xr.DataArray)
-    assert isinstance(output["tmax"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["ppt"].dims == ("y", "x", "time")
-    assert output["tmax"].dims == ("y", "x", "time")   
-
-    # check dates
-    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
-    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
-    
-    assert end_date1 - start_date1 == pd.Timedelta("0D")
-    assert end_date2 - start_date2 == pd.Timedelta("0D")
-    assert start_date1 - start_date2 == pd.Timedelta("0D")
-    assert end_date1 - end_date2 == pd.Timedelta("0D")
-
-    assert "ppt" in output["ppt"].time[0].values.item()
-    assert "tmax" in output["tmax"].time[0].values.item()
-    assert len(output["ppt"].time.values) == 1
-    assert len(output["tmax"].time.values) == 1
-
-def test_getDaymet(AOI):
-
-    varname = ["prcp", "tmax"]
-    startDate = "2018-01-01"
-    endDate   = "2018-01-02"
-    verbose   = True
-
-    # Call function to get output
-    output = climatePy.getDaymet(AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"prcp", "tmax"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["prcp"], xr.DataArray)
-    assert isinstance(output["tmax"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["prcp"].dims == ("y", "x", "time")
-    assert output["tmax"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["prcp"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["prcp"].time[1].values.item()).group(0), "%Y-%m-%d")
-    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["tmax"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["tmax"].time[1].values.item()).group(0), "%Y-%m-%d")
-
-    assert end_date1 - start_date1 == pd.Timedelta("1D")
-    assert end_date2 - start_date2 == pd.Timedelta("1D")
-
-def test_getLivneh_monthly_case1(AOI):
-    verbose   = True
-    varname="wind"
-    startDate="2010-01-01"
-    endDate="2010-02-01"
-    timeRes="monthly"
-
-    # Call function to get output
-    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"wind"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["wind"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["wind"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[1].values.item()).group(0), "%Y-%m-%d")
-
-    assert end_date1 - start_date1 == pd.Timedelta("29D")
-    
-    assert "wind" in output["wind"].time[0].values.item()
-    assert len(output["wind"].time.values) == 2
-
-
-def test_getLivneh_monthly_case2(AOI):
-
-    verbose   = True
-    varname="wind"
-    startDate="2010-01-01"
-	endDate="2010-01-01"
-	timeRes="monthly"
-
-    # Call function to get output
-    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"wind"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["wind"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["wind"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    assert end_date1 - start_date1 == pd.Timedelta("0D")
-    
-    assert "wind" in output["wind"].time[0].values.item()
-    assert len(output["wind"].time.values) == 1
-
-
-def test_getLivneh_daily_case1(AOI):
-
-    verbose   = True
-    varname   = "wind"
-    startDate = "2010-01-01"
-    endDate   = "2010-01-01"
-    timeRes   = "daily"
-
-    # Call function to get output
-    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"wind"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["wind"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["wind"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    assert end_date1 - start_date1 == pd.Timedelta("0D")
-    
-    assert "wind" in output["wind"].time[0].values.item()
-    assert len(output["wind"].time.values) == 1
-
-def test_getLivneh_daily_case2(AOI):
-
-    verbose   = True
-    varname   = "wind"
-    startDate = "2010-01-01"
-    endDate   = "2010-02-04"
-	timeRes   = "daily"
-
-    # Call function to get output
-    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"wind"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["wind"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["wind"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[-1].values.item()).group(0), "%Y-%m-%d")
-    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[1].values.item()).group(0), "%Y-%m-%d")
-
-    assert end_date1 - start_date1 == pd.Timedelta("34D")
-    assert end_date2 - start_date1 == pd.Timedelta("1D")
-    
-    assert "wind" in output["wind"].time[0].values.item()
-    assert len(output["wind"].time.values) == 35
-
-    
-def test_getLivneh_fluxes_case1(AOI):
-
-    verbose   = True
-    varname   = "Baseflow"
-    startDate = "2010-01-01"
-    endDate   = "2010-01-02"
-
-    # Call function to get output
-    output = climatePy.getLivneh_fluxes(AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"Baseflow"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["Baseflow"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["Baseflow"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["Baseflow"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["Baseflow"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("1D")
-
-    # check data has correct start/end dates
-    assert start_date1.strftime("%Y-%m-%d") == startDate
-    assert end_date1.strftime("%Y-%m-%d") == endDate
-
-    assert "Baseflow" in output["Baseflow"].time[0].values.item()
-    assert len(output["Baseflow"].time.values) == 2
-
-def test_getLivneh_fluxes_case2(AOI):
-
-    verbose   = True
-    varname   = ["GroundHeat", "SWE"]
-    startDate = "2010-01-01"
-    endDate   = "2010-01-04"
-
-    # Call function to get output
-    output = climatePy.getLivneh_fluxes(AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"GroundHeat", "SWE"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["GroundHeat"], xr.DataArray)
-    assert isinstance(output["SWE"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["GroundHeat"].dims == ("y", "x", "time")
-    assert output["SWE"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["GroundHeat"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["GroundHeat"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["SWE"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["SWE"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("3D")
-    assert end_date2 - start_date2 == pd.Timedelta("3D")
-    assert start_date2 - start_date1 == pd.Timedelta("0D")
-    assert end_date2 - end_date1 == pd.Timedelta("0D")
-
-    # check data has correct start/end dates
-    assert start_date1.strftime("%Y-%m-%d") == startDate
-    assert end_date1.strftime("%Y-%m-%d") == endDate
-    assert start_date2.strftime("%Y-%m-%d") == startDate
-    assert end_date2.strftime("%Y-%m-%d") == endDate
-
-    assert "GroundHeat" in output["GroundHeat"].time[0].values.item()
-    assert "SWE" in output["SWE"].time[0].values.item()
-    
-    assert len(output["GroundHeat"].time.values) == 4
-    assert len(output["SWE"].time.values) == 4
-
-def test_getLivneh_fluxes_case3(AOI):
-
-    verbose   = True
-    varname   = ["LatentHeat"]
-    startDate = "2010-01-01"
-    endDate   = "2010-02-02"
-
-    # Call function to get output
-    output = climatePy.getLivneh_fluxes(AOI, varname, startDate, endDate, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"LatentHeat"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["LatentHeat"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["LatentHeat"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["LatentHeat"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["LatentHeat"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("32D")
-
-    # check data has correct start/end dates
-    assert start_date1.strftime("%Y-%m-%d") == startDate
-    assert end_date1.strftime("%Y-%m-%d") == endDate
-
-    assert "LatentHeat" in output["LatentHeat"].time[0].values.item()
-    
-    assert len(output["LatentHeat"].time.values) == 33
-
-def test_getPolaris_case1(AOI):
-    # ---- Case 1: single variable as list ----
-    verbose   = True
-    varname   = ["mean alpha 5-15cm"]
-	# varname = "p95 theta_s 100-200cm"
-    
-    # Call function to get output
-    output = climatePy.getPolaris(AOI, varname, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"mean alpha 5-15cm"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["mean alpha 5-15cm"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["mean alpha 5-15cm"].dims == ("y", "x")
-
-    # check CRS
-    assert output["mean alpha 5-15cm"].crs == "EPSG:4326"
-
-    # check dimensions
-    assert len(output["mean alpha 5-15cm"]) == 3238
-
-    # assert output["mean alpha 5-15cm"].shape == (3238, 7078)
-    
-def test_getPolaris_case2(AOI):
-    # ---- Case 2: single variable as string ----
-    verbose   = True
-	varname = "p95 theta_s 100-200cm"
-
-    # Call function to get output
-    output = climatePy.getPolaris(AOI, varname, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"p95 theta_s 100-200cm"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["p95 theta_s 100-200cm"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["p95 theta_s 100-200cm"].dims == ("y", "x")
-
-    # check CRS
-    assert output["p95 theta_s 100-200cm"].crs == "EPSG:4326"
-
-    # check dimensions
-    assert len(output["p95 theta_s 100-200cm"]) == 3238
-
-    # assert output["p95 theta_s 100-200cm"].shape == (3238, 7078)
-
-
-def test_getPolaris_case3(AOI):
-    # ---- Case 3: multiple variables ----
-    verbose   = True
-    varname   = ["mean clay 100-200cm", "p95 theta_s 100-200cm"]
-
-    # TODO: problem with "mean ksat 100-200cm" varname, probably more issues with other datasets as well...
-    # varname = ["mean ksat 100-200cm"]
-
-    # Call function to get output
-    output = climatePy.getPolaris(AOI, varname, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {'mean clay 100-200cm', 'p95 theta_s 100-200cm'}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["p95 theta_s 100-200cm"], xr.DataArray)
-    assert isinstance(output["mean clay 100-200cm"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["p95 theta_s 100-200cm"].dims == ("y", "x")
-    assert output["mean clay 100-200cm"].dims == ("y", "x")
-
-    # check CRS
-    assert output["p95 theta_s 100-200cm"].crs == "EPSG:4326"
-    assert output["mean clay 100-200cm"].crs == "EPSG:4326"
-
-    # check dimensions
-    assert len(output["p95 theta_s 100-200cm"]) == 3238
-    assert len(output["mean clay 100-200cm"]) == 3238
-    
-    # assert output["p95 theta_s 100-200cm"].shape == (3238, 7078)
-    # assert output["mean clay 100-200cm"].shape == (3238, 7078)
-
-def test_getMACA_month_case1(AOI):
-
-    # ---- Case 1: single variable as list ----
-    verbose   = True
-    varname   = ["pr"]
-    startDate = "2010-01-01"
-    endDate   = "2010-02-02"
-    timeRes   = "month"
-    # timeRes   = 'day'
-    model     = 'CCSM4'
-    scenario  = 'rcp45'
-
-    # Call function to get output
-    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"pr"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("31D")
-
-    startmonth = datetime.strptime(startDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
-    endmonth = datetime.strptime(endDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
-
-    # check data has correct start/end dates
-    assert start_date1.strftime("%Y-%m-%d") == startmonth
-    assert end_date1.strftime("%Y-%m-%d") == endmonth
-
-    assert "pr" in output["pr"].time[0].values.item()
-    
-    assert len(output["pr"].time.values) == 2
-
-def test_getMACA_month_case2(AOI):
-    
-    # ---- Case 1: single variable as list ----
-    verbose   = True
-    varname   = ["pr", "vpd"]
-    startDate = "2010-01-04"
-    endDate   = "2010-03-10"
-    timeRes   = "month"
-    # timeRes   = 'day'
-    model     = 'CCSM4'
-    scenario  = 'rcp45'
-
-    # Call function to get output
-    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"vpd", "pr"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-    assert isinstance(output["vpd"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-    assert output["vpd"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("59D")
-    assert end_date2 - start_date2 == pd.Timedelta("59D")
-
-    startmonth = datetime.strptime(startDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
-    endmonth = datetime.strptime(endDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
-
-    # check data has correct start/end dates
-    assert start_date1.strftime("%Y-%m-%d") == startmonth
-    assert end_date1.strftime("%Y-%m-%d") == endmonth
-    assert start_date2.strftime("%Y-%m-%d") == startmonth
-    assert end_date2.strftime("%Y-%m-%d") == endmonth
-
-    assert "pr" in output["pr"].time[0].values.item()
-    assert "vpd" in output["vpd"].time[0].values.item()
-
-    assert len(output["pr"].time.values) == 3
-    assert len(output["vpd"].time.values) == 3
-
-    # assert output['pr'].shape == (23, 48, 3)
-    # assert output['vpd'].shape == (23, 48, 3)
-
-def test_getMACA_day_case1(AOI):
-    #  ---- Case 1: Daily ----
-    verbose   = True
-    varname   = ["pr"]
-    startDate = "2010-01-01"
-    endDate   = "2010-01-02"
-    timeRes   = "day"
-    model     = 'CCSM4'
-    scenario  = 'rcp45'
-
-    # Call function to get output
-    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == { "pr"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("1D")
-
-
-    assert "pr" in output["pr"].time[0].values.item()
-
-    assert len(output["pr"].time.values) == 2
-
-    # assert output['pr'].shape == (23, 48, 2)
-
-def test_getMACA_day_case2(AOI):
-    #  ---- Case 2: Daily multi variable ----
-    verbose   = True
-    varname   = ["pr", "vpd"]
-    startDate = "2010-01-01"
-    endDate   = "2010-01-02"
-    timeRes   = "day"
-    model     = 'CCSM4'
-    scenario  = 'rcp45'
-
-    # Call function to get output
-    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"vpd", "pr"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["pr"], xr.DataArray)
-    assert isinstance(output["vpd"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["pr"].dims == ("y", "x", "time")
-    assert output["vpd"].dims == ("y", "x", "time")
-
-    # Assert that the temporal resolution of the output DataArrays is correct
-    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[0].values.item()).group(0), "%Y-%m-%d")
-    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[-1].values.item()).group(0), "%Y-%m-%d")
-
-    # check temporal range
-    assert end_date1 - start_date1 == pd.Timedelta("1D")
-    assert end_date2 - start_date2 == pd.Timedelta("1D")
-
-    assert "pr" in output["pr"].time[0].values.item()
-    assert "vpd" in output["vpd"].time[0].values.item()
-
-    assert len(output["pr"].time.values) == 2
-    assert len(output["vpd"].time.values) == 2
-    
-    # assert output['pr'].shape == (23, 48, 2)
-    # assert output['vpd'].shape == (23, 48, 2)
-
-def test_get3DEP_case1(AOI):
-    #  ---- Case 1: 30m DEM ----
-    verbose   = True
-    res       = '30m'
-
-    # Call function to get output
-    output = climatePy.get3DEP(AOI, res, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"elevation"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["elevation"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["elevation"].dims == ("y", "x")
-
-    assert output["elevation"].attrs['crs'] == "EPSG:4269"
-
-    assert len(output["elevation"]) == 3238
-    
-    # assert output['elevation'].shape == (3238, 7078)
-
-def test_get3DEP_case2(AOI):
-    #  ---- Case 2: 10m DEM ----
-    verbose   = True
-    res       = '10m'
-
-    # Call function to get output
-    output = climatePy.get3DEP(AOI, res, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"elevation"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["elevation"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["elevation"].dims == ("y", "x")
-
-    assert output["elevation"].attrs['crs'] == "EPSG:4269"
-    
-    assert len(output["elevation"]) == 9712
-    
-    # assert output['elevation'].shape == (9712, 21231)
-
-def test_getISRIC_soils_case1(AOI):
-    #  ---- Case 1: Vertisols ----
-    verbose   = True
-    varname       = 'Vertisols'
-
-    # Call function to get output
-    output = climatePy.getISRIC_soils(AOI, varname, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"Vertisols"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["Vertisols"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["Vertisols"].dims == ("y", "x")
-
-    assert output["Vertisols"].attrs['crs'] == "EPSG:4326"
-
-    assert len(output["Vertisols"]) == 432
-    
-    # assert output['Vertisols'].shape == (432, 945)
-
-
-def test_getISRIC_soils_case2(AOI):
-    #  ---- Case 2: Gypsisols ----
-    verbose   = True
-    varname       = 'Gypsisols'
-
-    # Call function to get output
-    output = climatePy.getISRIC_soils(AOI, varname, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"Gypsisols"}
-    
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["Gypsisols"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["Gypsisols"].dims == ("y", "x")
-
-    assert output["Gypsisols"].attrs['crs'] == "EPSG:4326"
-
-    assert len(output["Gypsisols"]) == 432
-    
-    # assert output['Gypsisols'].shape == (432, 945)
-
-def test_getISRIC_soils_case3(AOI):
-    # ---- Case 3: Multiple variables ----
-    verbose   = True
-    varname       = ['Vertisols', 'Gypsisols']
-
-    # Call function to get output
-    output = climatePy.getISRIC_soils(AOI, varname, verbose)
-
-    # Assert that the output is a dictionary
-    assert type(output) == dict
-
-    # Assert that the output dictionary has the correct keys
-    assert set(output.keys()) == {"Vertisols", "Gypsisols"}
-
-    # Assert that the values of the output dictionary are xarray DataArrays
-    assert isinstance(output["Vertisols"], xr.DataArray)
-    assert isinstance(output["Gypsisols"], xr.DataArray)
-
-    # Assert that the dimensions of the output DataArrays are correct
-    assert output["Vertisols"].dims == ("y", "x")
-    assert output["Gypsisols"].dims == ("y", "x")
-
-    assert output["Vertisols"].attrs['crs'] == "EPSG:4326"
-    assert output["Gypsisols"].attrs['crs'] == "EPSG:4326"
-
-    assert len(output["Vertisols"]) == 432
-    assert len(output["Gypsisols"]) == 432
-
-    # assert output['Vertisols'].shape == (432, 945)
-    # assert output['Gypsisols'].shape == (432, 945)
+# pytest library
+import pytest
+
+# import climatePy modules
+import climatePy
+
+# data manipulation libs
+import pandas as pd
+import geopandas as gpd
+import xarray as xr
+
+# standard python libs
+import re
+from datetime import datetime
+
+
+# old imports
+# from .climatePy import shortcuts
+# from src.climatePy import shortcuts
+# from src.climatePy import dap
+# from src.climatePy import climatepy_filter
+# from src.climatePy import utils
+
+# AOI    = gpd.read_file('climatePy/data/boulder_county.gpkg')
+# AOI    = gpd.read_file('climatePy/data/san_luis_obispo_county.gpkg')
+
+# @pytest.fixture(params=['miami_dade_county', 'san_luis_obispo_county', 
+#                         'litchfield_county', 'tuscaloosa_county', 
+#                         'boulder_county', 'king_county'])
+
+@pytest.fixture(params=['san_luis_obispo_county', 'boulder_county'])
+
+def AOI(request): 
+    # filepath = f'src/data/{request.param}.gpkg'
+    filepath = f'climatePy/data/{request.param}.gpkg'
+    AOI = gpd.read_file(filepath)
+    yield AOI
+
+def test_getTerraClim_case1(AOI):
+
+    varname = ["ppt", "tmax"]
+    startDate = "2018-01-01"
+    endDate   = "2018-03-02"
+    verbose   = True
+
+    # Call function to get output
+    output = climatePy.getTerraClim( AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"ppt", "tmax"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["ppt"], xr.DataArray)
+    assert isinstance(output["tmax"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["ppt"].dims == ("y", "x", "time")
+    assert output["tmax"].dims == ("y", "x", "time")   
+
+    dates1 = [datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values]
+    dates2 = [datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values]
+    
+    start_date1 = min(dates1)
+    end_date1   = max(dates1)
+    start_date2 = min(dates2)
+    end_date2   = max(dates2)
+
+    assert end_date1 - start_date1 == pd.Timedelta("59D")
+    assert end_date2 - start_date2 == pd.Timedelta("59D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+
+    assert "ppt" in output["ppt"].time[0].values.item()
+    assert "tmax" in output["tmax"].time[0].values.item()
+
+def test_getGridMET_case1(AOI):
+    # ---- Case 1 ----
+    verbose   = True
+    varname = "pr"
+    startDate="2000-01-01"
+    endDate="2000-01-01"
+    
+    # Call function to get output
+    output = climatePy.getGridMET( AOI, varname, startDate, endDate, verbose)
+    
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"pr"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
+    
+    assert end_date1 - start_date1 == pd.Timedelta("0D")
+
+    assert "pr" in output["pr"].time[0].values.item()
+    assert len(output["pr"].time.values) == 1
+
+def test_getGridMET_case2(AOI):    
+    # ---- Case 2 ----
+    verbose   = True
+    varname = ["pr", "tmmx"]
+    startDate = "2018-01-01"
+    endDate   = "2018-01-02"
+
+    # Call function to get output
+    output = climatePy.getGridMET( AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"tmmx", "pr"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+    assert isinstance(output["tmmx"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+    assert output["tmmx"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
+    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
+    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
+    
+    assert end_date1 - start_date1 == pd.Timedelta("1D")
+    assert end_date2 - start_date2 == pd.Timedelta("1D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+
+    assert "pr" in output["pr"].time[0].values.item()
+    assert "tmmx" in output["tmmx"].time[0].values.item()
+    assert len(output["pr"].time.values) == 2
+    assert len(output["tmmx"].time.values) == 2
+
+def test_getGridMET_case3(AOI):
+    # ---- Case 3 ----
+    verbose = True
+    varname = ["pr", "tmmx", "rmin"]
+    startDate = "2015-01-01"
+    endDate   = "2016-02-05"
+
+    # Call function to get output
+    output = climatePy.getGridMET( AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"tmmx", "pr", "rmin"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+    assert isinstance(output["tmmx"], xr.DataArray)
+    assert isinstance(output["rmin"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+    assert output["tmmx"].dims == ("y", "x", "time")
+    assert output["rmin"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["pr"].time.values])
+    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
+    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmmx"].time.values])
+    start_date3 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
+    end_date3   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
+
+    assert end_date1 - start_date1 == pd.Timedelta("400D")
+    assert end_date2 - start_date2 == pd.Timedelta("400D")
+    assert end_date3 - start_date3 == pd.Timedelta("400D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+    assert end_date3 - end_date2 == pd.Timedelta("0D")
+
+    assert "pr" in output["pr"].time[0].values.item()
+    assert "tmmx" in output["tmmx"].time[0].values.item()
+    assert "rmin" in output["rmin"].time[0].values.item()
+
+    assert len(output["pr"].time.values) == 401
+    assert len(output["tmmx"].time.values) == 401
+    assert len(output["rmin"].time.values) == 401
+    
+def test_getGridMET_case4(AOI):
+    # ---- Case 4 ----
+    verbose = True
+    varname = ["rmin"]
+    startDate = "2005-01-01"
+    endDate   = "2010-01-01"
+
+    # Call function to get output
+    output = climatePy.getGridMET(AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"rmin"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["rmin"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["rmin"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["rmin"].time.values])
+
+    assert end_date1 - start_date1 == pd.Timedelta("1826D")
+
+    assert "rmin" in output["rmin"].time[0].values.item()
+    assert len(output["rmin"].time.values) == 1827
+
+    
+def test_getTerraClimNormals_case1(AOI):
+    
+    # ---- Case 1 ----
+    verbose   = True
+    varname = ["ppt", "tmax"]
+    scenario  = '19611990'
+    month     = [1, 2]
+
+    # call function
+    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"ppt", "tmax"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["ppt"], xr.DataArray)
+    assert isinstance(output["tmax"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["ppt"].dims == ("y", "x", "time")
+    assert output["tmax"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    
+    assert end_date1 - start_date1 == pd.Timedelta("31D")
+    assert end_date2 - start_date2 == pd.Timedelta("31D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+
+    # check time variables names are correct
+    assert "ppt" in output["ppt"].time[0].values.item()
+    assert "tmax" in output["tmax"].time[0].values.item()
+    assert scenario in output["ppt"].time[0].values.item()
+    assert scenario in output["tmax"].time[0].values.item()
+    assert len(output["ppt"].time.values) == 2
+    assert len(output["tmax"].time.values) == 2
+
+def test_getTerraClimNormals_case2(AOI):
+
+    # ---- Case 2 ----
+    verbose   = True
+    varname = ["ppt", "tmax"]
+    scenario  = '19812010'
+    month     = [i for i in range(1, 13)]
+
+    # call function
+    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"ppt", "tmax"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["ppt"], xr.DataArray)
+    assert isinstance(output["tmax"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["ppt"].dims == ("y", "x", "time")
+    assert output["tmax"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    
+    assert end_date1 - start_date1 == pd.Timedelta("334D")
+    assert end_date2 - start_date2 == pd.Timedelta("334D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+
+    # check time variables names are correct
+    assert "ppt" in output["ppt"].time[0].values.item()
+    assert "tmax" in output["tmax"].time[0].values.item()
+    assert scenario in output["ppt"].time[0].values.item()
+    assert scenario in output["tmax"].time[0].values.item()
+    assert len(output["ppt"].time.values) == 12
+    assert len(output["tmax"].time.values) == 12
+
+def test_getTerraClimNormals_case3(AOI):
+    # ---- Case 3 ----
+    verbose   = True
+    varname = ["ppt", "tmax"]
+    scenario = '2C'
+    month     = [1, 3]
+
+    # call function
+    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"ppt", "tmax"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["ppt"], xr.DataArray)
+    assert isinstance(output["tmax"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["ppt"].dims == ("y", "x", "time")
+    assert output["tmax"].dims == ("y", "x", "time")
+
+    # Assert dates are correct
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    
+    assert end_date1 - start_date1 == pd.Timedelta("59D")
+    assert end_date2 - start_date2 == pd.Timedelta("59D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+
+    # check time variables names are correct
+    assert "ppt" in output["ppt"].time[0].values.item()
+    assert "tmax" in output["tmax"].time[0].values.item()
+    assert scenario in output["ppt"].time[0].values.item()
+    assert scenario in output["tmax"].time[0].values.item()
+    assert len(output["ppt"].time.values) == 3
+    assert len(output["tmax"].time.values) == 3
+    
+def test_getTerraClimNormals_case4(AOI):
+    # ---- Case 4 ----
+    verbose   = True
+    varname = ["ppt", "tmax"]
+    scenario = '4C'
+    month     = [1]
+    output = climatePy.getTerraClimNormals( AOI, varname, month, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"ppt", "tmax"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["ppt"], xr.DataArray)
+    assert isinstance(output["tmax"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["ppt"].dims == ("y", "x", "time")
+    assert output["tmax"].dims == ("y", "x", "time")   
+
+    # check dates
+    start_date1 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    end_date1   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["ppt"].time.values])
+    start_date2 = min([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    end_date2   = max([datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', i).group(0), "%Y-%m-%d") for i in output["tmax"].time.values])
+    
+    assert end_date1 - start_date1 == pd.Timedelta("0D")
+    assert end_date2 - start_date2 == pd.Timedelta("0D")
+    assert start_date1 - start_date2 == pd.Timedelta("0D")
+    assert end_date1 - end_date2 == pd.Timedelta("0D")
+
+    assert "ppt" in output["ppt"].time[0].values.item()
+    assert "tmax" in output["tmax"].time[0].values.item()
+    assert len(output["ppt"].time.values) == 1
+    assert len(output["tmax"].time.values) == 1
+
+def test_getDaymet(AOI):
+
+    varname = ["prcp", "tmax"]
+    startDate = "2018-01-01"
+    endDate   = "2018-01-02"
+    verbose   = True
+
+    # Call function to get output
+    output = climatePy.getDaymet(AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"prcp", "tmax"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["prcp"], xr.DataArray)
+    assert isinstance(output["tmax"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["prcp"].dims == ("y", "x", "time")
+    assert output["tmax"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["prcp"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["prcp"].time[1].values.item()).group(0), "%Y-%m-%d")
+    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["tmax"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["tmax"].time[1].values.item()).group(0), "%Y-%m-%d")
+
+    assert end_date1 - start_date1 == pd.Timedelta("1D")
+    assert end_date2 - start_date2 == pd.Timedelta("1D")
+
+def test_getLivneh_monthly_case1(AOI):
+    verbose   = True
+    varname="wind"
+    startDate="2010-01-01"
+    endDate="2010-02-01"
+    timeRes="monthly"
+
+    # Call function to get output
+    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"wind"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["wind"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["wind"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[1].values.item()).group(0), "%Y-%m-%d")
+
+    assert end_date1 - start_date1 == pd.Timedelta("29D")
+    
+    assert "wind" in output["wind"].time[0].values.item()
+    assert len(output["wind"].time.values) == 2
+
+
+def test_getLivneh_monthly_case2(AOI):
+
+    verbose   = True
+    varname="wind"
+    startDate="2010-01-01"
+	endDate="2010-01-01"
+	timeRes="monthly"
+
+    # Call function to get output
+    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"wind"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["wind"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["wind"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    assert end_date1 - start_date1 == pd.Timedelta("0D")
+    
+    assert "wind" in output["wind"].time[0].values.item()
+    assert len(output["wind"].time.values) == 1
+
+
+def test_getLivneh_daily_case1(AOI):
+
+    verbose   = True
+    varname   = "wind"
+    startDate = "2010-01-01"
+    endDate   = "2010-01-01"
+    timeRes   = "daily"
+
+    # Call function to get output
+    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"wind"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["wind"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["wind"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    assert end_date1 - start_date1 == pd.Timedelta("0D")
+    
+    assert "wind" in output["wind"].time[0].values.item()
+    assert len(output["wind"].time.values) == 1
+
+def test_getLivneh_daily_case2(AOI):
+
+    verbose   = True
+    varname   = "wind"
+    startDate = "2010-01-01"
+    endDate   = "2010-02-04"
+	timeRes   = "daily"
+
+    # Call function to get output
+    output = climatePy.getLivneh(AOI, varname, startDate, endDate, timeRes, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"wind"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["wind"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["wind"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[-1].values.item()).group(0), "%Y-%m-%d")
+    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["wind"].time[1].values.item()).group(0), "%Y-%m-%d")
+
+    assert end_date1 - start_date1 == pd.Timedelta("34D")
+    assert end_date2 - start_date1 == pd.Timedelta("1D")
+    
+    assert "wind" in output["wind"].time[0].values.item()
+    assert len(output["wind"].time.values) == 35
+
+    
+def test_getLivneh_fluxes_case1(AOI):
+
+    verbose   = True
+    varname   = "Baseflow"
+    startDate = "2010-01-01"
+    endDate   = "2010-01-02"
+
+    # Call function to get output
+    output = climatePy.getLivneh_fluxes(AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"Baseflow"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["Baseflow"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["Baseflow"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["Baseflow"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["Baseflow"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("1D")
+
+    # check data has correct start/end dates
+    assert start_date1.strftime("%Y-%m-%d") == startDate
+    assert end_date1.strftime("%Y-%m-%d") == endDate
+
+    assert "Baseflow" in output["Baseflow"].time[0].values.item()
+    assert len(output["Baseflow"].time.values) == 2
+
+def test_getLivneh_fluxes_case2(AOI):
+
+    verbose   = True
+    varname   = ["GroundHeat", "SWE"]
+    startDate = "2010-01-01"
+    endDate   = "2010-01-04"
+
+    # Call function to get output
+    output = climatePy.getLivneh_fluxes(AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"GroundHeat", "SWE"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["GroundHeat"], xr.DataArray)
+    assert isinstance(output["SWE"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["GroundHeat"].dims == ("y", "x", "time")
+    assert output["SWE"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["GroundHeat"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["GroundHeat"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["SWE"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["SWE"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("3D")
+    assert end_date2 - start_date2 == pd.Timedelta("3D")
+    assert start_date2 - start_date1 == pd.Timedelta("0D")
+    assert end_date2 - end_date1 == pd.Timedelta("0D")
+
+    # check data has correct start/end dates
+    assert start_date1.strftime("%Y-%m-%d") == startDate
+    assert end_date1.strftime("%Y-%m-%d") == endDate
+    assert start_date2.strftime("%Y-%m-%d") == startDate
+    assert end_date2.strftime("%Y-%m-%d") == endDate
+
+    assert "GroundHeat" in output["GroundHeat"].time[0].values.item()
+    assert "SWE" in output["SWE"].time[0].values.item()
+    
+    assert len(output["GroundHeat"].time.values) == 4
+    assert len(output["SWE"].time.values) == 4
+
+def test_getLivneh_fluxes_case3(AOI):
+
+    verbose   = True
+    varname   = ["LatentHeat"]
+    startDate = "2010-01-01"
+    endDate   = "2010-02-02"
+
+    # Call function to get output
+    output = climatePy.getLivneh_fluxes(AOI, varname, startDate, endDate, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"LatentHeat"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["LatentHeat"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["LatentHeat"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["LatentHeat"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["LatentHeat"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("32D")
+
+    # check data has correct start/end dates
+    assert start_date1.strftime("%Y-%m-%d") == startDate
+    assert end_date1.strftime("%Y-%m-%d") == endDate
+
+    assert "LatentHeat" in output["LatentHeat"].time[0].values.item()
+    
+    assert len(output["LatentHeat"].time.values) == 33
+
+def test_getPolaris_case1(AOI):
+    # ---- Case 1: single variable as list ----
+    verbose   = True
+    varname   = ["mean alpha 5-15cm"]
+	# varname = "p95 theta_s 100-200cm"
+    
+    # Call function to get output
+    output = climatePy.getPolaris(AOI, varname, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"mean alpha 5-15cm"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["mean alpha 5-15cm"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["mean alpha 5-15cm"].dims == ("y", "x")
+
+    # check CRS
+    assert output["mean alpha 5-15cm"].crs == "EPSG:4326"
+
+    # check dimensions
+    assert len(output["mean alpha 5-15cm"]) == 3238
+
+    # assert output["mean alpha 5-15cm"].shape == (3238, 7078)
+    
+def test_getPolaris_case2(AOI):
+    # ---- Case 2: single variable as string ----
+    verbose   = True
+	varname = "p95 theta_s 100-200cm"
+
+    # Call function to get output
+    output = climatePy.getPolaris(AOI, varname, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"p95 theta_s 100-200cm"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["p95 theta_s 100-200cm"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["p95 theta_s 100-200cm"].dims == ("y", "x")
+
+    # check CRS
+    assert output["p95 theta_s 100-200cm"].crs == "EPSG:4326"
+
+    # check dimensions
+    assert len(output["p95 theta_s 100-200cm"]) == 3238
+
+    # assert output["p95 theta_s 100-200cm"].shape == (3238, 7078)
+
+
+def test_getPolaris_case3(AOI):
+    # ---- Case 3: multiple variables ----
+    verbose   = True
+    varname   = ["mean clay 100-200cm", "p95 theta_s 100-200cm"]
+
+    # TODO: problem with "mean ksat 100-200cm" varname, probably more issues with other datasets as well...
+    # varname = ["mean ksat 100-200cm"]
+
+    # Call function to get output
+    output = climatePy.getPolaris(AOI, varname, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {'mean clay 100-200cm', 'p95 theta_s 100-200cm'}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["p95 theta_s 100-200cm"], xr.DataArray)
+    assert isinstance(output["mean clay 100-200cm"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["p95 theta_s 100-200cm"].dims == ("y", "x")
+    assert output["mean clay 100-200cm"].dims == ("y", "x")
+
+    # check CRS
+    assert output["p95 theta_s 100-200cm"].crs == "EPSG:4326"
+    assert output["mean clay 100-200cm"].crs == "EPSG:4326"
+
+    # check dimensions
+    assert len(output["p95 theta_s 100-200cm"]) == 3238
+    assert len(output["mean clay 100-200cm"]) == 3238
+    
+    # assert output["p95 theta_s 100-200cm"].shape == (3238, 7078)
+    # assert output["mean clay 100-200cm"].shape == (3238, 7078)
+
+def test_getMACA_month_case1(AOI):
+
+    # ---- Case 1: single variable as list ----
+    verbose   = True
+    varname   = ["pr"]
+    startDate = "2010-01-01"
+    endDate   = "2010-02-02"
+    timeRes   = "month"
+    # timeRes   = 'day'
+    model     = 'CCSM4'
+    scenario  = 'rcp45'
+
+    # Call function to get output
+    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"pr"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("31D")
+
+    startmonth = datetime.strptime(startDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
+    endmonth = datetime.strptime(endDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
+
+    # check data has correct start/end dates
+    assert start_date1.strftime("%Y-%m-%d") == startmonth
+    assert end_date1.strftime("%Y-%m-%d") == endmonth
+
+    assert "pr" in output["pr"].time[0].values.item()
+    
+    assert len(output["pr"].time.values) == 2
+
+def test_getMACA_month_case2(AOI):
+    
+    # ---- Case 1: single variable as list ----
+    verbose   = True
+    varname   = ["pr", "vpd"]
+    startDate = "2010-01-04"
+    endDate   = "2010-03-10"
+    timeRes   = "month"
+    # timeRes   = 'day'
+    model     = 'CCSM4'
+    scenario  = 'rcp45'
+
+    # Call function to get output
+    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"vpd", "pr"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+    assert isinstance(output["vpd"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+    assert output["vpd"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("59D")
+    assert end_date2 - start_date2 == pd.Timedelta("59D")
+
+    startmonth = datetime.strptime(startDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
+    endmonth = datetime.strptime(endDate, "%Y-%m-%d").replace(day=1).strftime("%Y-%m-%d")
+
+    # check data has correct start/end dates
+    assert start_date1.strftime("%Y-%m-%d") == startmonth
+    assert end_date1.strftime("%Y-%m-%d") == endmonth
+    assert start_date2.strftime("%Y-%m-%d") == startmonth
+    assert end_date2.strftime("%Y-%m-%d") == endmonth
+
+    assert "pr" in output["pr"].time[0].values.item()
+    assert "vpd" in output["vpd"].time[0].values.item()
+
+    assert len(output["pr"].time.values) == 3
+    assert len(output["vpd"].time.values) == 3
+
+    # assert output['pr'].shape == (23, 48, 3)
+    # assert output['vpd'].shape == (23, 48, 3)
+
+def test_getMACA_day_case1(AOI):
+    #  ---- Case 1: Daily ----
+    verbose   = True
+    varname   = ["pr"]
+    startDate = "2010-01-01"
+    endDate   = "2010-01-02"
+    timeRes   = "day"
+    model     = 'CCSM4'
+    scenario  = 'rcp45'
+
+    # Call function to get output
+    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == { "pr"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("1D")
+
+
+    assert "pr" in output["pr"].time[0].values.item()
+
+    assert len(output["pr"].time.values) == 2
+
+    # assert output['pr'].shape == (23, 48, 2)
+
+def test_getMACA_day_case2(AOI):
+    #  ---- Case 2: Daily multi variable ----
+    verbose   = True
+    varname   = ["pr", "vpd"]
+    startDate = "2010-01-01"
+    endDate   = "2010-01-02"
+    timeRes   = "day"
+    model     = 'CCSM4'
+    scenario  = 'rcp45'
+
+    # Call function to get output
+    output = climatePy.getMACA(AOI, varname, startDate, endDate,timeRes, model, scenario, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"vpd", "pr"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["pr"], xr.DataArray)
+    assert isinstance(output["vpd"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["pr"].dims == ("y", "x", "time")
+    assert output["vpd"].dims == ("y", "x", "time")
+
+    # Assert that the temporal resolution of the output DataArrays is correct
+    start_date1 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date1   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["pr"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    start_date2 = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[0].values.item()).group(0), "%Y-%m-%d")
+    end_date2   = datetime.strptime(re.search(r'\d{4}-\d{2}-\d{2}', output["vpd"].time[-1].values.item()).group(0), "%Y-%m-%d")
+
+    # check temporal range
+    assert end_date1 - start_date1 == pd.Timedelta("1D")
+    assert end_date2 - start_date2 == pd.Timedelta("1D")
+
+    assert "pr" in output["pr"].time[0].values.item()
+    assert "vpd" in output["vpd"].time[0].values.item()
+
+    assert len(output["pr"].time.values) == 2
+    assert len(output["vpd"].time.values) == 2
+    
+    # assert output['pr'].shape == (23, 48, 2)
+    # assert output['vpd'].shape == (23, 48, 2)
+
+def test_get3DEP_case1(AOI):
+    #  ---- Case 1: 30m DEM ----
+    verbose   = True
+    res       = '30m'
+
+    # Call function to get output
+    output = climatePy.get3DEP(AOI, res, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"elevation"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["elevation"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["elevation"].dims == ("y", "x")
+
+    assert output["elevation"].attrs['crs'] == "EPSG:4269"
+
+    assert len(output["elevation"]) == 3238
+    
+    # assert output['elevation'].shape == (3238, 7078)
+
+def test_get3DEP_case2(AOI):
+    #  ---- Case 2: 10m DEM ----
+    verbose   = True
+    res       = '10m'
+
+    # Call function to get output
+    output = climatePy.get3DEP(AOI, res, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"elevation"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["elevation"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["elevation"].dims == ("y", "x")
+
+    assert output["elevation"].attrs['crs'] == "EPSG:4269"
+    
+    assert len(output["elevation"]) == 9712
+    
+    # assert output['elevation'].shape == (9712, 21231)
+
+def test_getISRIC_soils_case1(AOI):
+    #  ---- Case 1: Vertisols ----
+    verbose   = True
+    varname       = 'Vertisols'
+
+    # Call function to get output
+    output = climatePy.getISRIC_soils(AOI, varname, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"Vertisols"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["Vertisols"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["Vertisols"].dims == ("y", "x")
+
+    assert output["Vertisols"].attrs['crs'] == "EPSG:4326"
+
+    assert len(output["Vertisols"]) == 432
+    
+    # assert output['Vertisols'].shape == (432, 945)
+
+
+def test_getISRIC_soils_case2(AOI):
+    #  ---- Case 2: Gypsisols ----
+    verbose   = True
+    varname       = 'Gypsisols'
+
+    # Call function to get output
+    output = climatePy.getISRIC_soils(AOI, varname, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"Gypsisols"}
+    
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["Gypsisols"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["Gypsisols"].dims == ("y", "x")
+
+    assert output["Gypsisols"].attrs['crs'] == "EPSG:4326"
+
+    assert len(output["Gypsisols"]) == 432
+    
+    # assert output['Gypsisols'].shape == (432, 945)
+
+def test_getISRIC_soils_case3(AOI):
+    # ---- Case 3: Multiple variables ----
+    verbose   = True
+    varname       = ['Vertisols', 'Gypsisols']
+
+    # Call function to get output
+    output = climatePy.getISRIC_soils(AOI, varname, verbose)
+
+    # Assert that the output is a dictionary
+    assert type(output) == dict
+
+    # Assert that the output dictionary has the correct keys
+    assert set(output.keys()) == {"Vertisols", "Gypsisols"}
+
+    # Assert that the values of the output dictionary are xarray DataArrays
+    assert isinstance(output["Vertisols"], xr.DataArray)
+    assert isinstance(output["Gypsisols"], xr.DataArray)
+
+    # Assert that the dimensions of the output DataArrays are correct
+    assert output["Vertisols"].dims == ("y", "x")
+    assert output["Gypsisols"].dims == ("y", "x")
+
+    assert output["Vertisols"].attrs['crs'] == "EPSG:4326"
+    assert output["Gypsisols"].attrs['crs'] == "EPSG:4326"
+
+    assert len(output["Vertisols"]) == 432
+    assert len(output["Gypsisols"]) == 432
+
+    # assert output['Vertisols'].shape == (432, 945)
+    # assert output['Gypsisols'].shape == (432, 945)
```

### Comparing `climatePy-0.0.4.1/tests/test_utils.py` & `climatePy-0.0.4.23/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# pytest library
-import pytest
-
-# import climatePy utils module
-import climatePy._utils as climatePy
-
-# standard python libs
-import re
-from datetime import datetime
-
-# old imports
-# from climatePy import utils
-# from src.climatePy import utils
-
-def test_getExtension():
-    # Test cases where the input string contains a file extension
-    assert climatePy.getExtension('myfile.txt') == 'txt'
-    assert climatePy.getExtension('my.file.with.multiple.dots.txt') == 'txt'
-    assert climatePy.getExtension('/path/to/myfile.txt') == 'txt'
-    assert climatePy.getExtension('/path/to/my.file.with.multiple.dots.txt') == 'txt'
-
-    # Test cases where the input string does not contain a file extension
-    assert climatePy.getExtension('myfile') == ''
-    assert climatePy.getExtension('mypath/myfile') == ''
-    assert climatePy.getExtension('mypath/myfile.') == ''
-    assert climatePy.getExtension('mypath/.myfile') == 'myfile'
-    assert climatePy.getExtension('') == ''
-
-def test_format_units():
-    # Test 1: No interval or unit string provided
-    assert climatePy.format_units() is None
-
-    # Test 2: Interval and unit strings are the same
-    assert climatePy.format_units("3 hours", "hours") == "3 hours"
-
-    assert climatePy.format_units("3 hours hours", "hours") == "3 hours"
-
-    # Test 3: Interval and unit strings are different
-    assert climatePy.format_units("2 weeks", "days") == "2 weeks"
-
-    assert climatePy.format_units("2 weeks weeks", "days") == "2 weeks weeks"
-
-    assert climatePy.format_units("2 weeks weeks", "weeks") == "2 weeks"
-    
-    # Test 4: Interval string contains multiple occurrences of unit string
-    assert climatePy.format_units("5 days days days", "days") == "5 days"
-
-    assert climatePy.format_units("5 days days days", "day") == '5 days days days'
-    
-    # Test 5: Interval string is a single word
-    assert climatePy.format_units("seconds", "seconds") == "seconds"
-
-    # Test 6: Interval string is a combination of words not containing unit string
-    assert climatePy.format_units("6 minutes and 30 seconds", "hours") == "6 minutes and 30 seconds"
-
-    assert climatePy.format_units("6 minutes and 30 seconds", "6 minutes and 30 seconds") == "6 minutes and 30 seconds"
-
-def test_format_date():
-    # Test case 1
-    date_str = '2022-03-12 09:30:00'
-    expected_output = '2022-03-12'
-    assert climatePy.format_date(date_str) == expected_output
-
-    # Test case 2
-    date_str = '2022-03-12T09:30:00'
-    expected_output = '2022-03-12'
-    assert climatePy.format_date(date_str) == expected_output
-
-    # Test case 3
-    date_str = '2022-03-12T09:30:00Z'
-    expected_output = '2022-03-12'
-    assert climatePy.format_date(date_str) == expected_output
-
-    # Test case 4
-    date_str = '2022-03-12T09:30:00-08:00'
-    expected_output = '2022-03-12'
-    assert climatePy.format_date(date_str) == expected_output
-
-    # Test case 5
-    date_str = '2022-03-12'
-    expected_output = '2022-03-12'
-    assert climatePy.format_date(date_str) == expected_output
-
-    # Test case 6
-    date_str = '2022-03-1' # Invalid date format
-    expected_output = ''
-    assert climatePy.format_date(date_str) == expected_output
+# pytest library
+import pytest
+
+# import climatePy utils module
+import climatePy._utils as climatePy
+
+# standard python libs
+import re
+from datetime import datetime
+
+# old imports
+# from climatePy import utils
+# from src.climatePy import utils
+
+def test_getExtension():
+    # Test cases where the input string contains a file extension
+    assert climatePy.getExtension('myfile.txt') == 'txt'
+    assert climatePy.getExtension('my.file.with.multiple.dots.txt') == 'txt'
+    assert climatePy.getExtension('/path/to/myfile.txt') == 'txt'
+    assert climatePy.getExtension('/path/to/my.file.with.multiple.dots.txt') == 'txt'
+
+    # Test cases where the input string does not contain a file extension
+    assert climatePy.getExtension('myfile') == ''
+    assert climatePy.getExtension('mypath/myfile') == ''
+    assert climatePy.getExtension('mypath/myfile.') == ''
+    assert climatePy.getExtension('mypath/.myfile') == 'myfile'
+    assert climatePy.getExtension('') == ''
+
+def test_format_units():
+    # Test 1: No interval or unit string provided
+    assert climatePy.format_units() is None
+
+    # Test 2: Interval and unit strings are the same
+    assert climatePy.format_units("3 hours", "hours") == "3 hours"
+
+    assert climatePy.format_units("3 hours hours", "hours") == "3 hours"
+
+    # Test 3: Interval and unit strings are different
+    assert climatePy.format_units("2 weeks", "days") == "2 weeks"
+
+    assert climatePy.format_units("2 weeks weeks", "days") == "2 weeks weeks"
+
+    assert climatePy.format_units("2 weeks weeks", "weeks") == "2 weeks"
+    
+    # Test 4: Interval string contains multiple occurrences of unit string
+    assert climatePy.format_units("5 days days days", "days") == "5 days"
+
+    assert climatePy.format_units("5 days days days", "day") == '5 days days days'
+    
+    # Test 5: Interval string is a single word
+    assert climatePy.format_units("seconds", "seconds") == "seconds"
+
+    # Test 6: Interval string is a combination of words not containing unit string
+    assert climatePy.format_units("6 minutes and 30 seconds", "hours") == "6 minutes and 30 seconds"
+
+    assert climatePy.format_units("6 minutes and 30 seconds", "6 minutes and 30 seconds") == "6 minutes and 30 seconds"
+
+def test_format_date():
+    # Test case 1
+    date_str = '2022-03-12 09:30:00'
+    expected_output = '2022-03-12'
+    assert climatePy.format_date(date_str) == expected_output
+
+    # Test case 2
+    date_str = '2022-03-12T09:30:00'
+    expected_output = '2022-03-12'
+    assert climatePy.format_date(date_str) == expected_output
+
+    # Test case 3
+    date_str = '2022-03-12T09:30:00Z'
+    expected_output = '2022-03-12'
+    assert climatePy.format_date(date_str) == expected_output
+
+    # Test case 4
+    date_str = '2022-03-12T09:30:00-08:00'
+    expected_output = '2022-03-12'
+    assert climatePy.format_date(date_str) == expected_output
+
+    # Test case 5
+    date_str = '2022-03-12'
+    expected_output = '2022-03-12'
+    assert climatePy.format_date(date_str) == expected_output
+
+    # Test case 6
+    date_str = '2022-03-1' # Invalid date format
+    expected_output = ''
+    assert climatePy.format_date(date_str) == expected_output
```

