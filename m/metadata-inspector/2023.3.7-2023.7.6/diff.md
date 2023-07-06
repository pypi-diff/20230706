# Comparing `tmp/metadata_inspector-2023.3.7.tar.gz` & `tmp/metadata_inspector-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadata_inspector-2023.3.7.tar", last modified: Tue Mar  7 19:38:17 2023, max compression
+gzip compressed data, was "metadata_inspector-2023.7.6.tar", last modified: Thu Jul  6 12:08:50 2023, max compression
```

## Comparing `metadata_inspector-2023.3.7.tar` & `metadata_inspector-2023.7.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-07 19:38:17.428990 metadata_inspector-2023.3.7/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1516 2022-10-05 16:26:44.000000 metadata_inspector-2023.3.7/LICENSE
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2416 2023-03-07 19:38:17.428990 metadata_inspector-2023.3.7/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1304 2022-10-12 08:55:23.000000 metadata_inspector-2023.3.7/README.md
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       38 2023-03-07 19:38:17.428990 metadata_inspector-2023.3.7/setup.cfg
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2648 2022-11-17 09:45:21.000000 metadata_inspector-2023.3.7/setup.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-07 19:38:17.425657 metadata_inspector-2023.3.7/src/
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-07 19:38:17.425657 metadata_inspector-2023.3.7/src/metadata_inspector/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     7133 2023-03-07 19:38:06.000000 metadata_inspector-2023.3.7/src/metadata_inspector/__init__.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     3978 2023-03-07 19:38:06.000000 metadata_inspector-2023.3.7/src/metadata_inspector/_slk.py
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       58 2023-03-07 19:38:06.000000 metadata_inspector-2023.3.7/src/metadata_inspector/_version.py
-drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-03-07 19:38:17.428990 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2416 2023-03-07 19:38:17.000000 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/PKG-INFO
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      405 2023-03-07 19:38:17.000000 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)        1 2023-03-07 19:38:17.000000 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       62 2023-03-07 19:38:17.000000 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/entry_points.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)      226 2023-03-07 19:38:17.000000 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/requires.txt
--rw-r--r--   0 wilfred   (1000) wilfred   (1001)       19 2023-03-07 19:38:17.000000 metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1516 2022-10-05 16:26:44.000000 metadata_inspector-2023.7.6/LICENSE
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2416 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/PKG-INFO
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     1304 2022-10-12 08:55:23.000000 metadata_inspector-2023.7.6/README.md
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)       38 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/setup.cfg
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2673 2023-07-05 07:58:41.000000 metadata_inspector-2023.7.6/setup.py
+drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/src/
+drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/src/metadata_inspector/
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     7735 2023-07-06 09:23:24.000000 metadata_inspector-2023.7.6/src/metadata_inspector/__init__.py
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     6041 2023-07-06 09:23:24.000000 metadata_inspector-2023.7.6/src/metadata_inspector/_slk.py
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)       58 2023-07-06 09:23:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector/_version.py
+drwxr-xr-x   0 wilfred   (1000) wilfred   (1001)        0 2023-07-06 12:08:50.918263 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)     2416 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)      405 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)        1 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)       62 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)      240 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/requires.txt
+-rw-r--r--   0 wilfred   (1000) wilfred   (1001)       19 2023-07-06 12:08:50.000000 metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/top_level.txt
```

### Comparing `metadata_inspector-2023.3.7/LICENSE` & `metadata_inspector-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata_inspector-2023.3.7/PKG-INFO` & `metadata_inspector-2023.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata_inspector
-Version: 2023.3.7
+Version: 2023.7.6
 Summary: Inspect metadata of weather/climate datasets
 Home-page: https://github.com/FREVA-CLINT/metadata-inspektor.git
 Author: Martin Bergemann
 Author-email: bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/FREVA-CLINT/metadata-inspektor
```

### Comparing `metadata_inspector-2023.3.7/README.md` & `metadata_inspector-2023.7.6/README.md`

 * *Files identical despite different names*

### Comparing `metadata_inspector-2023.3.7/setup.py` & `metadata_inspector-2023.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     entry_points={"console_scripts": ["metadata-inspector = metadata_inspector:cli"]},
     install_requires=[
         "cftime",
         "dask[diagnostics]",
         "hurry.filesize",
         "h5netcdf",
         "netCDF4",
+        "numpy>=1.20.3",
         "requests",
         "xarray",
     ],
     extras_require={
         "tests": [
             "black",
             "pytest",
```

### Comparing `metadata_inspector-2023.3.7/src/metadata_inspector/__init__.py` & `metadata_inspector-2023.7.6/src/metadata_inspector/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Metadata inspector."""
 from __future__ import annotations
 import argparse
 from functools import partial
 from pathlib import Path
+import json
 import warnings
 import sys
 from typing import Optional, TextIO
 
 from cftime import num2date
 from dask import array as dask_array
 from hurry.filesize import alternative, size
 import numpy as np
 import xarray as xr
-import yaml
 
 from ._version import __version__
 from ._slk import get_slk_metadata, login
 
 
 def _summarize_datavar(name: str, var: xr.DataArray, col_width: int) -> str:
     out = [
@@ -68,30 +68,31 @@
     )
     parsed_args = app.parse_args(args)
     return parsed_args.input, parsed_args.html
 
 
 def dataset_from_hsm(input_file: str) -> xr.Dataset:
     """Create a dataset view from attributes."""
-
-    attrs: dict[str, dict[str, str]] = (
-        yaml.safe_load(get_slk_metadata(input_file)) or {}
-    ).get("Keywords", {})
-
-    dset = xr.Dataset({}, attrs=attrs.pop("global"))
-    for dim in attrs.pop("dims"):
+    global_attrs: dict[str, dict[str, str]] = get_slk_metadata(input_file)
+    attrs = json.loads(global_attrs.pop("document", {}).pop("Keywords", "{}"))
+    nc_attrs = {}
+    for key in ("netcdf", "netcdf_header"):
+        for k, value in global_attrs.get(key, {}).items():
+            nc_attrs[k] = value
+    dset = xr.Dataset({}, attrs=attrs.pop("global", {}) or nc_attrs)
+    for dim in attrs.pop("dims", []):
         size = int(attrs[dim].pop("size"))
         start, end = float(attrs[dim].pop("start")), float(
             attrs[dim].pop("end")
         )
         vec = np.linspace(start, end, size)
         if dim == "time":
             vec = num2date(vec, attrs[dim]["units"], attrs[dim]["calendar"])
         dset[dim] = xr.DataArray(vec, name=dim, dims=(dim,), attrs=attrs[dim])
-    for data_var in attrs.pop("data_vars"):
+    for data_var in attrs.pop("data_vars", []):
         dims = attrs[data_var].pop("dims")
         sizes = [dset[d].size for d in dims]
         dset[data_var] = xr.DataArray(
             dask_array.empty(sizes),
             name=data_var,
             dims=dims,
             attrs=attrs[data_var],
@@ -107,45 +108,52 @@
     extensions: tuple[str, ...] = (
         ".nc",
         ".nc4",
         ".grb",
         ".grib",
         ".grib2",
         ".grb2",
-        ".zarr",
         ".h5",
         ".hdf5",
     )
     for inp_file in input_:
-        inp = inp_file.expanduser().absolute()
-        if inp.is_dir() and inp.exists():
+        schema, _, path = str(inp_file).partition(":")
+        if not path:
+            path = schema
+        inp = Path(path).expanduser().absolute()
+        if schema in ("hsm", "slk") or inp.parts[1] == "arch":
+            files_archive.append(str(inp))
+        if inp.exists() and inp.suffix in (".zarr",):
+            files_fs.append(str(inp))
+        elif inp.is_dir() and inp.exists():
             files_fs += [
                 str(inp_file)
                 for inp_file in inp.rglob("*")
                 if inp_file.suffix.lower() in extensions
             ]
         elif inp.is_file() and inp.exists():
             files_fs.append(str(inp))
         elif inp.parent.exists() and inp.parent.is_dir():
             files_fs += [
                 str(inp_file)
                 for inp_file in inp.parent.rglob(inp.name)
                 if inp_file.suffix in extensions
             ]
-        elif inp.parts[1] == "arch" or str(inp).startswith("slk:"):
-            files_archive.append(str(inp))
     return sorted(files_fs), sorted(files_archive)
 
 
 def _open_datasets(files_fs: list[str], files_hsm: list[str]) -> xr.Dataset:
     dsets: list[xr.Dataset] = []
     if files_fs:
         dsets.append(
             xr.open_mfdataset(
-                files_fs, parallel=False, combine="by_coords", use_cftime=True
+                files_fs,
+                parallel=False,
+                combine="by_coords",
+                use_cftime=True,
             )
         )
     if files_hsm:
         login()
         for inp_file in files_hsm:
             dsets.append(dataset_from_hsm(inp_file))
     return xr.merge(dsets)
@@ -158,15 +166,15 @@
     ----------
 
     input_files: list[Path]
         Collection of input files that are to be inspected
     html: bool, default: True
         If true a representation suitable for html is displayed.
     """
-
+    xr.core.formatting.EMPTY_REPR = "    *not enough information for display*"
     files_fs, files_hsm = _get_files(input_files)
     if not files_fs and not files_hsm:
         return "No files found", sys.stderr
     try:
         dset = _open_datasets(files_fs, files_hsm)
     except Exception as error:
         error_header = (
@@ -181,15 +189,18 @@
                 "do not use the --html flag.</p>"
             )
             return msg, sys.stdout
 
         else:
             msg = f"{error_header}\n{error_msg}"
             return msg, sys.stderr
-    fsize = size(dset.nbytes, system=alternative)
+    if dset.nbytes == 0:
+        fsize = dset.attrs.pop("file_size", "unkown")
+    else:
+        fsize = size(dset.nbytes, system=alternative)
     if html:
         out_str = xr.core.formatting_html.dataset_repr(dset)
     else:
         xr.core.options.OPTIONS["display_expand_data_vars"] = True
         xr.core.options.OPTIONS["display_expand_attrs"] = True
         xr.core.options.OPTIONS["display_expand_data"] = True
         xr.core.options.OPTIONS["display_max_rows"] = 100
@@ -197,15 +208,15 @@
             xr.core.formatting._mapping_repr,
             title="Data variables",
             summarizer=_summarize_datavar,
             expand_option_name="display_expand_data_vars",
         )
         out_str = xr.core.formatting.dataset_repr(dset)
     replace_str = (
-        ("xarray.Dataset", f"Dataset (byte-size: {fsize})"),
+        ("xarray.Dataset", f"Dataset (dataset-size: {fsize})"),
         (
             "<svg class='icon xr-icon-file-text2'>",
             "<i class='fa fa-file-text-o'>",
         ),
         ("<svg class='icon xr-icon-database'>", "<i class='fa fa-database'>"),
         ("</use></svg>", "</use></i>"),
         ("numpy.", ""),
```

### Comparing `metadata_inspector-2023.3.7/src/metadata_inspector.egg-info/PKG-INFO` & `metadata_inspector-2023.7.6/src/metadata_inspector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata-inspector
-Version: 2023.3.7
+Version: 2023.7.6
 Summary: Inspect metadata of weather/climate datasets
 Home-page: https://github.com/FREVA-CLINT/metadata-inspektor.git
 Author: Martin Bergemann
 Author-email: bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/FREVA-CLINT/metadata-inspektor
```

