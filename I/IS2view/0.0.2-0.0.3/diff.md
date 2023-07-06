# Comparing `tmp/IS2view-0.0.2.tar.gz` & `tmp/IS2view-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IS2view-0.0.2.tar", last modified: Thu Jun  8 16:26:31 2023, max compression
+gzip compressed data, was "IS2view-0.0.3.tar", last modified: Thu Jul  6 19:35:59 2023, max compression
```

## Comparing `IS2view-0.0.2.tar` & `IS2view-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 16:26:31.413514 IS2view-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 16:26:31.409514 IS2view-0.0.2/IS2view/
--rw-r--r--   0 runner    (1001) docker     (122)    75103 2023-06-08 16:26:17.000000 IS2view-0.0.2/IS2view/IS2view.py
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-06-08 16:26:17.000000 IS2view-0.0.2/IS2view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-06-08 16:26:17.000000 IS2view-0.0.2/IS2view/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-06-08 16:26:17.000000 IS2view-0.0.2/IS2view/io.py
--rw-r--r--   0 runner    (1001) docker     (122)    45988 2023-06-08 16:26:17.000000 IS2view-0.0.2/IS2view/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-06-08 16:26:17.000000 IS2view-0.0.2/IS2view/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 16:26:31.409514 IS2view-0.0.2/IS2view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-06-08 16:26:31.000000 IS2view-0.0.2/IS2view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-06-08 16:26:31.000000 IS2view-0.0.2/IS2view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 16:26:31.000000 IS2view-0.0.2/IS2view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-08 16:26:31.000000 IS2view-0.0.2/IS2view.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-08 16:26:31.000000 IS2view-0.0.2/IS2view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-08 16:26:17.000000 IS2view-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-08 16:26:17.000000 IS2view-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3790 2023-06-08 16:26:31.409514 IS2view-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2967 2023-06-08 16:26:17.000000 IS2view-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-08 16:26:17.000000 IS2view-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 16:26:31.413514 IS2view-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1757 2023-06-08 16:26:17.000000 IS2view-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:35:59.993704 IS2view-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-06 19:35:49.000000 IS2view-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-06 19:35:49.000000 IS2view-0.0.3/CONTRIBUTORS.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:35:59.993704 IS2view-0.0.3/IS2view/
+-rw-r--r--   0 runner    (1001) docker     (122)      588 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66749 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3766 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14581 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46061 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-06 19:35:49.000000 IS2view-0.0.3/IS2view/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:35:59.993704 IS2view-0.0.3/IS2view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3427 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-06 19:35:59.000000 IS2view-0.0.3/IS2view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-07-06 19:35:49.000000 IS2view-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-06 19:35:49.000000 IS2view-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3427 2023-07-06 19:35:59.993704 IS2view-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-06 19:35:49.000000 IS2view-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-07-06 19:35:49.000000 IS2view-0.0.3/postBuild
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-06 19:35:49.000000 IS2view-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-06 19:35:49.000000 IS2view-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-06 19:35:59.993704 IS2view-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2184 2023-07-06 19:35:49.000000 IS2view-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-07-06 19:35:49.000000 IS2view-0.0.3/version.txt
```

### Comparing `IS2view-0.0.2/IS2view/IS2view.py` & `IS2view-0.0.3/IS2view/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 #!/usr/bin/env python
 u"""
-IS2view.py
-Written by Tyler Sutterley (12/2022)
-Jupyter notebook, user interface and plotting tools for visualizing
-    rioxarray variables on leaflet maps
+api.py
+Written by Tyler Sutterley (07/2023)
+Plotting tools for visualizing rioxarray variables on leaflet maps
 
 PYTHON DEPENDENCIES:
-    numpy: Scientific Computing Tools For Python
-        https://numpy.org
-        https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
+    geopandas: Python tools for geographic data
+        http://geopandas.readthedocs.io/
     ipywidgets: interactive HTML widgets for Jupyter notebooks and IPython
         https://ipywidgets.readthedocs.io/en/latest/
     ipyleaflet: Jupyter / Leaflet bridge enabling interactive maps
         https://github.com/jupyter-widgets/ipyleaflet
     matplotlib: Python 2D plotting library
         http://matplotlib.org/
         https://github.com/matplotlib/matplotlib
+    numpy: Scientific Computing Tools For Python
+        https://numpy.org
+        https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
+    OWSLib: Pythonic interface for Open Geospatial Consortium (OGC) web services
+        https://owslib.readthedocs.io/
     rasterio: Access to geospatial raster data
         https://github.com/rasterio/rasterio
         https://rasterio.readthedocs.io
     xarray: N-D labeled arrays and datasets in Python
         https://docs.xarray.dev/en/stable/
 
 UPDATE HISTORY:
+    Updated 07/2023: renamed module from IS2view.py to api.py
+        add plot functions for map basemaps and added geometries
+        add imshow function for visualizing current leaflet map
+    Updated 06/2023: moved widgets functions to separate moddule
     Updated 12/2022: added case for warping input image
     Updated 11/2022: modifications for dask-chunked rasters
     Written 07/2022
 """
 import io
 import os
 import copy
@@ -38,14 +45,20 @@
 import numpy as np
 import collections.abc
 from traitlets import HasTraits, Float, Tuple, observe
 from traitlets.utils.bunch import Bunch
 
 # attempt imports
 try:
+    import geopandas as gpd
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("geopandas not available")
+    warnings.warn("Some functions will throw an exception if called")
+try:
     import ipywidgets
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("ipywidgets not available")
     warnings.warn("Some functions will throw an exception if called")
 try:
     import ipyleaflet
@@ -60,14 +73,20 @@
     import matplotlib.pyplot as plt
     import matplotlib.colors as colors
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("matplotlib not available")
     warnings.warn("Some functions will throw an exception if called")
 try:
+    import owslib.wms
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("owslib not available")
+    warnings.warn("Some functions will throw an exception if called")
+try:
     import rasterio.transform
     import rasterio.warp
 except (ImportError, ModuleNotFoundError) as exc:
     warnings.filterwarnings("module")
     warnings.warn("rasterio not available")
     warnings.warn("Some functions will throw an exception if called")
 try:
@@ -78,383 +97,14 @@
     warnings.warn("Some functions will throw an exception if called")
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # set environmental variable for anonymous s3 access
 os.environ['AWS_NO_SIGN_REQUEST'] = 'YES'
 
-class widgets:
-    def __init__(self, **kwargs):
-        # set default keyword options
-        kwargs.setdefault('loglevel', logging.CRITICAL)
-        kwargs.setdefault('directory', os.getcwd())
-        kwargs.setdefault('style', {})
-        # set logging level
-        logging.basicConfig(level=kwargs['loglevel'])
-        # set style
-        self.style = copy.copy(kwargs['style'])
-
-        # dropdown menu for setting asset
-        asset_list = ['nsidc-https','nsidc-s3','atlas-s3','atlas-local']
-        self.asset = ipywidgets.Dropdown(
-            options=asset_list,
-            value='nsidc-https',
-            description='Asset:',
-            description_tooltip=("Asset: Location to get the data\n\t"
-                "nsidc-https: NSIDC on-prem DAAC\n\t"
-                "nsidc-s3: NSIDC Cumulus s3 bucket`\n\t"
-                "atlas-s3: s3 bucket in `us-west-2`\n\t"
-                "atlas-local: local directory"),
-            disabled=False,
-            style=self.style,
-        )
-
-        # working data directory if local
-        self.directory = ipywidgets.Text(
-            value=kwargs['directory'],
-            description='Directory:',
-            description_tooltip=("Directory: working data directory"),
-            disabled=False,
-            style=self.style,
-        )
-        self.directory.layout.display = 'none'
-
-        # dropdown menu for setting ATL14/15 release
-        release_list = ['001','002']
-        self.release = ipywidgets.Dropdown(
-            options=release_list,
-            value='002',
-            description='Release:',
-            description_tooltip=("Release: ATL14/15 data release\n\t"
-                "001: Release-01\n\t"
-                "002: Release-02"),
-            disabled=False,
-            style=self.style,
-        )
-
-        # dropdown menu for setting ATL14/15 region
-        region_list = ['AA', 'CN', 'CS', 'GL', 'IS', 'RA', 'SV']
-        self.region = ipywidgets.Dropdown(
-            options=region_list,
-            description='Region:',
-            description_tooltip=("Region: ATL14/15 region\n\t"
-                "AA: Antarctica\n\t"
-                "CN: Northern Canadian Archipelago\n\t"
-                "CS: Southern Canadian Archipelago\n\t"
-                "GL: Greenland\n\t"
-                "IS: Iceland\n\t"
-                "SV: Svalbard\n\t"
-                "RA: Russian High Arctic"),
-            disabled=False,
-            style=self.style,
-        )
-
-        # dropdown menu for setting ATL15 resolution
-        resolution_list = ['01km', '10km', '20km', '40km']
-        self.resolution = ipywidgets.Dropdown(
-            options=resolution_list,
-            description='Resolution:',
-            description_tooltip=("Resolution: ATL15 resolution\n\t"
-                "01km: 1 kilometer horizontal\n\t"
-                "10km: 10 kilometers horizontal\n\t"
-                "20km: 20 kilometers horizontal\n\t"
-                "40km: 40 kilometers horizontal"),
-            disabled=False,
-            style=self.style,
-        )
-
-        # dropdown menu for selecting group to read from file
-        # use Release-01 groups as the initial default
-        group_list = ['delta_h', 'dhdt_lag1', 'dhdt_lag4', 'dhdt_lag8']
-        self.group = ipywidgets.Dropdown(
-            options=group_list,
-            description='Group:',
-            description_tooltip="Group: ATL15 data group to read from file",
-            disabled=False,
-            style=self.style,
-        )
-
-        # dropdown menu for selecting data format
-        format_list = ['nc', 'zarr']
-        self.format = ipywidgets.Dropdown(
-            options=format_list,
-            description='Format:',
-            description_tooltip=("Format: ATL15 data format\n\t"
-                "nc: Native netCDF4\n\t"
-                "zarr: Cloud-optimized zarr"),
-            disabled=False,
-            style=self.style,
-        )
-        self.format.layout.display = 'none'
-
-        # dropdown menu for selecting variable to draw on map
-        variable_list = ['delta_h', 'dhdt']
-        self.variable = ipywidgets.Dropdown(
-            options=variable_list,
-            description='Variable:',
-            description_tooltip="Variable: variable to display on leaflet map",
-            disabled=False,
-            style=self.style,
-        )
-
-        # dropdown menu for selecting time lag to draw on map
-        self.timelag = ipywidgets.IntSlider(
-            description='Lag:',
-            description_tooltip="Lag: time lag to draw on leaflet map",
-            disabled=False,
-            style=self.style,
-        )
-
-        # Reverse the colormap
-        self.dynamic = ipywidgets.Checkbox(
-            value=False,
-            description='Dynamic',
-            description_tooltip=("Dynamic: Dynamically set normalization range"),
-            disabled=False,
-            style=self.style,
-        )
-
-        # watch widgets for changes
-        self.asset.observe(self.set_directory_visibility)
-        self.asset.observe(self.set_format_visibility)
-        self.release.observe(self.set_groups)
-        self.dynamic.observe(self.set_dynamic)
-        self.variable.observe(self.set_lag_visibility)
-
-        # slider for normalization range
-        self.range = ipywidgets.FloatRangeSlider(
-            min = -10,
-            max = 10,
-            value = [-5, 5],
-            description='Range:',
-            description_tooltip=("Range: Plot normalization range"),
-            disabled=False,
-            continuous_update=False,
-            orientation='horizontal',
-            readout=True,
-            style=self.style,
-        )
-
-        # all listed colormaps in matplotlib version
-        cmap_set = set(cm.datad.keys()) | set(cm.cmaps_listed.keys())
-        # colormaps available in this program
-        # (no reversed, qualitative or miscellaneous)
-        self.cmaps_listed = {}
-        self.cmaps_listed['Perceptually Uniform Sequential'] = [
-            'viridis', 'plasma', 'inferno', 'magma', 'cividis']
-        self.cmaps_listed['Sequential'] = ['Greys', 'Purples',
-            'Blues', 'Greens', 'Oranges', 'Reds', 'YlOrBr', 'YlOrRd',
-            'OrRd', 'PuRd', 'RdPu', 'BuPu', 'GnBu', 'PuBu', 'YlGnBu',
-            'PuBuGn', 'BuGn', 'YlGn']
-        self.cmaps_listed['Sequential (2)'] = ['binary', 'gist_yarg',
-            'gist_gray', 'gray', 'bone', 'pink', 'spring', 'summer',
-            'autumn', 'winter', 'cool', 'Wistia', 'hot', 'afmhot',
-            'gist_heat', 'copper']
-        self.cmaps_listed['Diverging'] = ['PiYG', 'PRGn', 'BrBG',
-            'PuOr', 'RdGy', 'RdBu', 'RdYlBu', 'RdYlGn', 'Spectral',
-            'coolwarm', 'bwr', 'seismic']
-        self.cmaps_listed['Cyclic'] = ['twilight',
-            'twilight_shifted', 'hsv']
-        # create list of available colormaps in program
-        cmap_list = []
-        for val in self.cmaps_listed.values():
-            cmap_list.extend(val)
-        # reduce colormaps to available in program and matplotlib
-        cmap_set &= set(cmap_list)
-        # dropdown menu for setting colormap
-        self.cmap = ipywidgets.Dropdown(
-            options=sorted(cmap_set),
-            value='viridis',
-            description='Colormap:',
-            description_tooltip=("Colormap: matplotlib colormaps "
-                "for displayed variable"),
-            disabled=False,
-            style=self.style,
-        )
-
-        # Reverse the colormap
-        self.reverse = ipywidgets.Checkbox(
-            value=False,
-            description='Reverse Colormap',
-            description_tooltip=("Reverse Colormap: reverse matplotlib "
-                "colormap for displayed variable"),
-            disabled=False,
-            style=self.style,
-        )
-
-    @property
-    def projection(self):
-        """return string for map projection based on region
-        """
-        projections = {}
-        projections['AA'] = 'South'
-        projections['CN'] = 'North'
-        projections['CS'] = 'North'
-        projections['GL'] = 'North'
-        projections['IS'] = 'North'
-        projections['SV'] = 'North'
-        projections['RA'] = 'North'
-        return projections[self.region.value]
-
-    @property
-    def center(self):
-        """return default central point latitude and longitude
-        for map based on region
-        """
-        centers = {}
-        centers['AA'] = (-90.0, 0.0)
-        centers['CN'] = (79.0, -85.0)
-        centers['CS'] = (70.0, -73.0)
-        centers['GL'] = (72.5, -45.0)
-        centers['IS'] = (64.5, -18.5)
-        centers['SV'] = (79.0, 19.0)
-        centers['RA'] = (79.0, 78.0)
-        return centers[self.region.value]
-
-    @property
-    def zoom(self):
-        """return default zoom level for map based on region
-        """
-        zooms = {}
-        zooms['AA'] = 1
-        zooms['CN'] = 2
-        zooms['CS'] = 2
-        zooms['GL'] = 1
-        zooms['IS'] = 3
-        zooms['SV'] = 3
-        zooms['RA'] = 2
-        return zooms[self.region.value]
-
-    @property
-    def _r(self):
-        """return string for reversed Matplotlib colormaps
-        """
-        cmap_reverse_flag = '_r' if self.reverse.value else ''
-        return cmap_reverse_flag
-
-    @property
-    def colormap(self):
-        """return string for Matplotlib colormaps
-        """
-        return self.cmap.value + self._r
-
-    @property
-    def vmin(self):
-        """return minimum of normalization range
-        """
-        return self.range.value[0]
-
-    @property
-    def vmax(self):
-        """return maximum of normalization range
-        """
-        return self.range.value[1]
-
-    def set_directory_visibility(self, sender):
-        """updates the visibility of the directory widget
-        """
-        if (self.asset.value == 'atlas-local'):
-            self.directory.layout.display = 'inline-flex'
-        else:
-            self.directory.layout.display = 'none'
-
-    def set_format_visibility(self, sender):
-        """updates the visibility of the data format widget
-        """
-        if self.asset.value in ('atlas-s3','atlas-local'):
-            self.format.layout.display = 'inline-flex'
-        else:
-            self.format.layout.display = 'none'
-            # set the format back to the default
-            self.format.value = 'nc'
-
-    def set_atl14_defaults(self, *args, **kwargs):
-        """sets the default widget parameters for ATL14 variables
-        """
-        # use dynamic normalization
-        self.dynamic.value = True
-
-    def set_atl15_defaults(self, *args, **kwargs):
-        """sets the default widget parameters for ATL15 variables
-        """
-        group = copy.copy(self.group.value)
-        variables = {}
-        variables['delta_h'] = 'delta_h'
-        variables['dhdt_lag1'] = 'dhdt'
-        # set annual time lags
-        # extend possible time lags to 16 years post-launch
-        for timelag in range(4, 68, 4):
-            variables[f'dhdt_lag{timelag:d}'] = 'dhdt'
-        # set default variable for group
-        self.variable.value = variables[group]
-
-    def set_groups(self, sender):
-        """sets the list of available groups for a release
-        """
-        group_list = ['delta_h', 'dhdt_lag1', 'dhdt_lag4', 'dhdt_lag8']
-        # append lag12 group
-        if (int(self.release.value) > 1):
-            group_list.append('dhdt_lag12')
-        # set group list
-        self.group.options = group_list
-
-    def set_variables(self, *args):
-        """sets the list of available variables in a group
-        """
-        if any(args):
-            # set list of available variables
-            self.variable.options = sorted(args[0].keys())
-        else:
-            # return to temporary defaults
-            self.variable.options = ['delta_h', 'dhdt']
-
-    def set_dynamic(self, *args, **kwargs):
-        """sets variable normalization range if dynamic
-        """
-        if self.dynamic.value:
-            self.range.min = -100
-            self.range.max = 100
-            self.range.value = [np.nan, np.nan]
-            self.range.layout.display = 'none'
-        else:
-            self.range.min = -10
-            self.range.max = 10
-            self.range.value = [-5, 5]
-            self.range.layout.display = 'inline-flex'
-
-    def set_lags(self, ds):
-        """sets available time range for lags
-        """
-        self.timelag.value = 1
-        self.timelag.min = 1
-        # try setting the max lag
-        try:
-            self.timelag.max = len(ds['time'])
-        except Exception as exc:
-            self.timelag.max = 1
-
-    def set_lag_visibility(self, sender):
-        """updates the visibility of the time lag widget
-        """
-        # list of invariant parameters
-        invariant_parameters = ['ice_mask']
-        if (int(self.release.value) <= 1):
-            invariant_parameters.append('cell_area')
-        # check if setting an invariant variable
-        if self.variable.value in invariant_parameters:
-            self.timelag.layout.display = 'none'
-        else:
-            self.timelag.layout.display = 'inline-flex'
-
-    @property
-    def lag(self):
-        """return the 0-based index for the time lag
-        """
-        return self.timelag.value - 1
-
 # map projections
 projections = {}
 projections['EPSG:3857'] = dict(name='EPSG3857', custom=False),
 projections['EPSG:3413'] = dict(
     name='EPSG:3413',
     custom=True,
     proj4def="""+proj=stere +lat_0=90 +lat_ts=70 +lon_0=-45 +k=1 +x_0=0 +y_0=0
@@ -516,15 +166,15 @@
         url='https://elevation2.arcgis.com/arcgis/rest/services/Polar/AntarcticDEM/ImageServer',
         crs=projections['EPSG:3031']
     )
 except (NameError, AttributeError):
     pass
 
 # draw ipyleaflet map
-class leaflet:
+class Leaflet:
     """Create interactive leaflet maps for visualizing ATL14/15 data
 
     Parameters
     ----------
     map : obj or NoneType, default None
         ``ipyleaflet.Map``
     attribution : bool, default False
@@ -716,15 +366,15 @@
         filename : str
             Output GeoJSON filename
         kwargs : dict, default {}
             Additional attributes for the GeoJSON file
         """
         # dump the geometries to a geojson file
         kwargs.update(self.geometries)
-        with open(filename, 'w') as fid:
+        with open(filename, mode='w') as fid:
             json.dump(kwargs, fid)
         # print the filename and dictionary structure
         logging.info(filename)
         logging.info(list(kwargs.keys()))
 
     def add(self, obj):
         """wrapper function for adding layers and controls to leaflet maps
@@ -768,14 +418,78 @@
             except ipyleaflet.LayerException as exc:
                 logging.info(f"{obj} already removed from map")
                 pass
             except ipyleaflet.ControlException as exc:
                 logging.info(f"{obj} already removed from map")
                 pass
 
+    # plot basemap
+    def plot_basemap(self, ax=None, **kwargs):
+        """Plot the current basemap
+
+        Parameters
+        ----------
+        ax: obj, default None
+            Figure axis
+        kwargs: dict, default {}
+            Additional keyword arguments for ``wms.getmap``
+        """
+        # set default keyword arguments
+        kwargs.setdefault('layers', ['BlueMarble_NextGeneration'])
+        kwargs.setdefault('format', 'image/png')
+        kwargs.setdefault('srs', self.map.crs['name'])
+        # create figure axis if non-existent
+        if (ax is None):
+            _, ax = plt.subplots()
+        # get the pixel bounds and resolution of the map
+        (left, top), (right, bottom) = self.map.pixel_bounds
+        resolution = self.map.crs['resolutions'][int(self.map.zoom)]
+        # calculate the size of the map in pixels
+        kwargs.setdefault('size', [int((right-left)), int((bottom-top))])
+        # calculate the bounding box of the map in projected coordinates
+        bbox = [None]*4
+        bbox[0] = self.map.crs['origin'][0] + left*resolution
+        bbox[1] = self.map.crs['origin'][1] - bottom*resolution
+        bbox[2] = self.map.crs['origin'][0] + right*resolution
+        bbox[3] = self.map.crs['origin'][1] - top*resolution
+        kwargs.setdefault('bbox', bbox)
+        # create WMS request for basemap image at bounds and resolution
+        srs = kwargs['srs'].replace(':', '').lower()
+        url = f'https://gibs.earthdata.nasa.gov/wms/{srs}/best/wms.cgi?'
+        wms = owslib.wms.WebMapService(url=url, version='1.1.1')
+        basemap = wms.getmap(**kwargs)
+        # read WMS layer and plot
+        img = plt.imread(io.BytesIO(basemap.read()))
+        ax.imshow(img, extent=[bbox[0],bbox[2],bbox[1],bbox[3]])
+
+    # plot geometries
+    def plot_geometries(self, ax=None, **kwargs):
+        """Plot the current geometries in the coordinate reference
+        system (``crs``) of the map
+
+        Parameters
+        ----------
+        ax: obj, default None
+            Figure axis
+        kwargs: dict, default {}
+            Additional keyword arguments for ``plot``
+        """
+        # return if no geometries
+        if (len(self.geometries['features']) == 0):
+            return
+        # create figure axis if non-existent
+        if (ax is None):
+            _, ax = plt.subplots()
+        # create a geopandas GeoDataFrame from the geometries
+        # convert coordinate reference system to map crs
+        gdf = gpd.GeoDataFrame.from_features(self.geometries,
+            crs=self.geometries['crs']).to_crs(self.crs)
+        # create plot with all geometries
+        gdf.plot(ax=ax, **kwargs)
+
     @property
     def layers(self):
         """get the map layers
         """
         return self.map.layers
 
     @property
@@ -1295,15 +1009,14 @@
         self._data = self._ds_selected.sel(x=x, y=y, method='nearest').values[0]
         self._units = self._ds[self._variable].attrs['units']
         # only create popup if valid
         if np.isnan(self._data):
             return
         # create contextual popup
         child = ipywidgets.HTML()
-        print(np.squeeze(self._data), self._units)
         child.value = '{0:0.1f} {1}'.format(np.squeeze(self._data), self._units)
         self.popup = ipyleaflet.Popup(location=(lat, lon),
             child=child, name='popup')
         self.add(self.popup)
 
     # add colorbar widget to leaflet map
     def add_colorbar(self, **kwargs):
@@ -1349,14 +1062,50 @@
         output = ipywidgets.Image(value=png.getvalue(), format='png')
         self.colorbar = ipyleaflet.WidgetControl(widget=output,
             transparent_bg=True, position=kwargs['position'])
         # add colorbar
         self.add(self.colorbar)
         plt.close()
 
+    # save the current map as an image
+    def imshow(self, ax=None, **kwargs):
+        """Save the current map as a static image
+
+        Parameters
+        ----------
+        ax: obj, default None
+            Figure axis
+        kwargs: dict, default {}
+            Additional keyword arguments for ``imshow``
+        """
+        # create figure axis if non-existent
+        if (ax is None):
+            _, ax = plt.subplots()
+        # extract units
+        longname = self._ds[self._variable].attrs['long_name'].replace('  ', ' ')
+        units = self._ds[self._variable].attrs['units'][0]
+        # clip image to map bounds
+        visible = self.clip_image(self._ds_selected)
+        # color bar keywords
+        cbar_kwargs = dict(label=f'{longname} [{units}]', orientation='horizontal')
+        visible.plot.imshow(ax=ax,
+            norm=self.norm,
+            interpolation="nearest",
+            cmap=self.cmap,
+            alpha=self.opacity,
+            add_colorbar=True,
+            add_labels=True,
+            cbar_kwargs=cbar_kwargs,
+            **kwargs
+        )
+        # set image extent
+        ax.set_xlim(self.extent[0], self.extent[1])
+        ax.set_ylim(self.extent[2], self.extent[3])
+        ax.set_aspect('equal', adjustable='box')
+
 @xr.register_dataset_accessor('timeseries')
 class TimeSeries(HasTraits):
     """A xarray.DataArray extension for extracting and plotting a time series
 
     Parameters
     ----------
     ds : obj
```

### Comparing `IS2view-0.0.2/IS2view/__init__.py` & `IS2view-0.0.3/IS2view/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ==========================================
 
 Interactive visualization and data extraction tool for the
 ICESat-2 ATL14/15 Gridded Land Ice Height Products
 
 Documentation is available at https://is2view.readthedocs.io
 """
-from IS2view.IS2view import widgets, leaflet, layers, image_service_layer
-from IS2view.convert import convert
-from IS2view.io import from_file, from_rasterio, from_xarray
 import IS2view.utilities
 import IS2view.version
-# get version
+from IS2view.api import Leaflet, layers, image_service_layer
+from IS2view.convert import convert
+from IS2view.io import from_file, from_rasterio, from_xarray
+from IS2view.tools import widgets
+# get semantic version from setuptools-scm
 __version__ = IS2view.version.version
```

### Comparing `IS2view-0.0.2/IS2view/convert.py` & `IS2view-0.0.3/IS2view/convert.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.2/IS2view/io.py` & `IS2view-0.0.3/IS2view/io.py`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.2/IS2view/utilities.py` & `IS2view-0.0.3/IS2view/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 utilities.py
 Written by Tyler Sutterley (06/2023)
 Download and management utilities
 
 UPDATE HISTORY:
     Updated 06/2023: using pathlib to define and expand paths
         add functions to retrieve and revoke NASA Earthdata User tokens
+        updated netCDF4 request type for NSIDC s3 bucket CMR queries
     Updated 12/2022: functions for managing and maintaining git repositories
     Updated 11/2022: can query for zarr datasets
     Updated 10/2022: public release of NSIDC s3 access
     Written 07/2022
 """
 from __future__ import print_function, division, annotations
 
@@ -1244,16 +1245,16 @@
     endpoint = {}
     endpoint['nsidc-s3'] = 's3'
     endpoint['atlas-s3'] = 's3'
     endpoint['nsidc-https'] = 'data'
     endpoint['atlas-local'] = 'data'
     # CMR request types
     request_type = {}
-    request_type['nsidc-s3'] = 'application/netcdf'
-    request_type['atlas-s3'] = 'application/netcdf'
+    request_type['nsidc-s3'] = 'application/x-netcdf'
+    request_type['atlas-s3'] = 'application/x-netcdf'
     request_type['nsidc-https'] = 'application/netcdf'
     request_type['atlas-local'] = 'application/netcdf'
 
     # attempt to get resource
     granule = None
     try:
         # query CMR
```

### Comparing `IS2view-0.0.2/IS2view.egg-info/PKG-INFO` & `IS2view-0.0.3/IS2view.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =======
 IS2view
 =======
 
@@ -48,27 +50,22 @@
 - https://icesat-2.gsfc.nasa.gov
 - https://icesat-2-scf.gsfc.nasa.gov
 - https://nsidc.org/data/icesat-2/
 
 Dependencies
 ############
 
-- `boto3: Amazon Web Services (AWS) SDK for Python <https://boto3.amazonaws.com/v1/documentation/api/latest/index.html>`_
-- `bottleneck: Fast NumPy array functions written in C <https://github.com/pydata/bottleneck>`_
-- `dask: Parallel computing with task scheduling <https://www.dask.org/>`_
-- `h5netcdf: Pythonic interface to netCDF4 via h5py <https://h5netcdf.org/>`_
 - `ipyleaflet: Interactive maps in the Jupyter notebook <https://ipyleaflet.readthedocs.io/en/latest/>`_
 - `matplotlib: Python 2D plotting library <https://matplotlib.org/>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
 - `rasterio: Access to geospatial raster data <https://rasterio.readthedocs.io/en/latest/>`_
 - `rioxarray: geospatial xarray extension powered by rasterio <https://github.com/corteva/rioxarray>`_
-- `s3fs: Pythonic file interface to S3 built on top of botocore <https://s3fs.readthedocs.io/en/latest/>`_
+- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm>`_
 - `xarray: N-D labeled arrays and datasets in Python <https://docs.xarray.dev/en/stable/>`_
-- `zarr: Chunked, compressed, N-dimensional arrays in Python <https://zarr.readthedocs.io/en/stable/>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/IS2view
 | A zip archive of the latest version is available directly at:
```

### Comparing `IS2view-0.0.2/LICENSE` & `IS2view-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `IS2view-0.0.2/PKG-INFO` & `IS2view-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: IS2view
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interactive visualization and data extraction tool for the ICESat-2 ATL14/15 Gridded Land Ice Height Products
 Home-page: https://github.com/tsutterley/IS2view
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2,elevation,digital elevation models,ipython,jupyter,graphics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 =======
 IS2view
 =======
 
@@ -48,27 +50,22 @@
 - https://icesat-2.gsfc.nasa.gov
 - https://icesat-2-scf.gsfc.nasa.gov
 - https://nsidc.org/data/icesat-2/
 
 Dependencies
 ############
 
-- `boto3: Amazon Web Services (AWS) SDK for Python <https://boto3.amazonaws.com/v1/documentation/api/latest/index.html>`_
-- `bottleneck: Fast NumPy array functions written in C <https://github.com/pydata/bottleneck>`_
-- `dask: Parallel computing with task scheduling <https://www.dask.org/>`_
-- `h5netcdf: Pythonic interface to netCDF4 via h5py <https://h5netcdf.org/>`_
 - `ipyleaflet: Interactive maps in the Jupyter notebook <https://ipyleaflet.readthedocs.io/en/latest/>`_
 - `matplotlib: Python 2D plotting library <https://matplotlib.org/>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
 - `rasterio: Access to geospatial raster data <https://rasterio.readthedocs.io/en/latest/>`_
 - `rioxarray: geospatial xarray extension powered by rasterio <https://github.com/corteva/rioxarray>`_
-- `s3fs: Pythonic file interface to S3 built on top of botocore <https://s3fs.readthedocs.io/en/latest/>`_
+- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm>`_
 - `xarray: N-D labeled arrays and datasets in Python <https://docs.xarray.dev/en/stable/>`_
-- `zarr: Chunked, compressed, N-dimensional arrays in Python <https://zarr.readthedocs.io/en/stable/>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/IS2view
 | A zip archive of the latest version is available directly at:
```

### Comparing `IS2view-0.0.2/README.rst` & `IS2view-0.0.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -28,27 +28,22 @@
 - https://icesat-2.gsfc.nasa.gov
 - https://icesat-2-scf.gsfc.nasa.gov
 - https://nsidc.org/data/icesat-2/
 
 Dependencies
 ############
 
-- `boto3: Amazon Web Services (AWS) SDK for Python <https://boto3.amazonaws.com/v1/documentation/api/latest/index.html>`_
-- `bottleneck: Fast NumPy array functions written in C <https://github.com/pydata/bottleneck>`_
-- `dask: Parallel computing with task scheduling <https://www.dask.org/>`_
-- `h5netcdf: Pythonic interface to netCDF4 via h5py <https://h5netcdf.org/>`_
 - `ipyleaflet: Interactive maps in the Jupyter notebook <https://ipyleaflet.readthedocs.io/en/latest/>`_
 - `matplotlib: Python 2D plotting library <https://matplotlib.org/>`_
 - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
 - `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
 - `rasterio: Access to geospatial raster data <https://rasterio.readthedocs.io/en/latest/>`_
 - `rioxarray: geospatial xarray extension powered by rasterio <https://github.com/corteva/rioxarray>`_
-- `s3fs: Pythonic file interface to S3 built on top of botocore <https://s3fs.readthedocs.io/en/latest/>`_
+- `setuptools_scm: manager for python package versions using scm metadata <https://pypi.org/project/setuptools-scm>`_
 - `xarray: N-D labeled arrays and datasets in Python <https://docs.xarray.dev/en/stable/>`_
-- `zarr: Chunked, compressed, N-dimensional arrays in Python <https://zarr.readthedocs.io/en/stable/>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/IS2view
 | A zip archive of the latest version is available directly at:
```

### Comparing `IS2view-0.0.2/setup.py` & `IS2view-0.0.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,27 @@
 else:
     # get install requirements
     with open('requirements.txt', mode='r', encoding='utf8') as fh:
         install_requires = [line.split().pop(0) for line in fh.read().splitlines()]
 
 # get version
 with open('version.txt', mode='r', encoding='utf8') as fh:
-    version = fh.read()
+    fallback_version = fh.read()
+
+# semantic version configuration for setuptools-scm
+setup_requires = ["setuptools_scm"]
+use_scm_version = {
+    "relative_to": __file__,
+    "local_scheme": "node-and-date",
+    "version_scheme": "python-simplified-semver",
+    "fallback_version":fallback_version,
+}
 
 setup(
     name='IS2view',
-    version=version,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     url='https://github.com/tsutterley/IS2view',
     author='Tyler Sutterley',
     author_email='tsutterl@uw.edu',
     license='MIT',
@@ -38,13 +46,17 @@
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Physics',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
     ],
     keywords=keywords,
     packages=find_packages(),
     install_requires=install_requires,
+    setup_requires=setup_requires,
+    use_scm_version=use_scm_version,
     include_package_data=True,
 )
```

