# Comparing `tmp/mikro-0.3.81.tar.gz` & `tmp/mikro-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mikro-0.3.81.tar", max compression
+gzip compressed data, was "mikro-0.3.9.tar", max compression
```

## Comparing `mikro-0.3.81.tar` & `mikro-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,23 @@
--rw-r--r--   0        0        0      497 2023-05-04 11:33:38.864146 mikro-0.3.81/mikro/__init__.py
--rw-r--r--   0        0        0       38 2022-11-21 13:25:24.312569 mikro-0.3.81/mikro/api/__init__.py
--rw-r--r--   0        0        0   411009 2023-06-12 09:55:46.068438 mikro-0.3.81/mikro/api/schema.py
--rw-r--r--   0        0        0        0 2022-11-21 13:19:21.452118 mikro-0.3.81/mikro/builders.py
--rw-r--r--   0        0        0        0 2023-01-24 14:42:54.553770 mikro-0.3.81/mikro/cli/__init__.py
--rw-r--r--   0        0        0     3237 2023-03-09 16:01:04.382912 mikro-0.3.81/mikro/cli/main.py
--rw-r--r--   0        0        0    92815 2023-01-24 15:15:30.502724 mikro-0.3.81/mikro/cli/schemas/v1.graphql
--rw-r--r--   0        0        0      166 2023-03-09 13:07:49.776971 mikro-0.3.81/mikro/cli/utils.py
--rw-r--r--   0        0        0        0 2022-08-25 14:13:51.564206 mikro-0.3.81/mikro/contrib/__init__.py
--rw-r--r--   0        0        0        0 2022-02-03 16:40:05.361043 mikro-0.3.81/mikro/contrib/fakts/__init__.py
--rw-r--r--   0        0        0     1303 2022-11-21 13:24:56.296558 mikro-0.3.81/mikro/contrib/fakts/datalayer.py
--rw-r--r--   0        0        0     9060 2023-05-31 07:31:29.070469 mikro-0.3.81/mikro/datalayer.py
--rw-r--r--   0        0        0      156 2022-03-21 13:01:57.991994 mikro-0.3.81/mikro/errors.py
--rw-r--r--   0        0        0     1174 2023-04-13 10:19:19.375180 mikro-0.3.81/mikro/funcs.py
--rw-r--r--   0        0        0      830 2023-05-04 11:33:08.291989 mikro-0.3.81/mikro/items.py
--rw-r--r--   0        0        0       92 2022-03-21 13:01:58.083994 mikro-0.3.81/mikro/links/__init__.py
--rw-r--r--   0        0        0     2574 2023-02-27 14:55:12.024266 mikro-0.3.81/mikro/links/datalayer.py
--rw-r--r--   0        0        0        0 2022-05-17 11:20:06.504915 mikro-0.3.81/mikro/links/errors.py
--rw-r--r--   0        0        0     1081 2023-03-04 14:55:46.173689 mikro-0.3.81/mikro/mikro.py
--rw-r--r--   0        0        0     1649 2023-01-19 09:09:28.169699 mikro-0.3.81/mikro/rath.py
--rw-r--r--   0        0        0    14412 2023-06-12 10:09:46.191178 mikro-0.3.81/mikro/scalars.py
--rw-r--r--   0        0        0     8085 2023-07-06 09:45:46.324713 mikro-0.3.81/mikro/structures.py
--rw-r--r--   0        0        0        0 2023-03-04 15:06:28.973785 mikro-0.3.81/mikro/testing/__init__.py
--rw-r--r--   0        0        0     1225 2023-03-04 15:22:43.161911 mikro-0.3.81/mikro/testing/datalayer.py
--rw-r--r--   0        0        0    12346 2023-06-07 08:20:53.944356 mikro-0.3.81/mikro/traits.py
--rw-r--r--   0        0        0     1314 2023-05-19 13:15:39.685195 mikro-0.3.81/mikro/utils.py
--rw-r--r--   0        0        0     1462 2023-06-27 13:36:16.567325 mikro-0.3.81/mikro/widgets.py
--rw-r--r--   0        0        0     1760 2023-07-06 16:56:46.935407 mikro-0.3.81/pyproject.toml
--rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 mikro-0.3.81/PKG-INFO
+-rw-r--r--   0        0        0      101 2022-08-25 11:10:14.051638 mikro-0.3.9/mikro/__init__.py
+-rw-r--r--   0        0        0       38 2022-11-21 13:25:24.312569 mikro-0.3.9/mikro/api/__init__.py
+-rw-r--r--   0        0        0   242929 2022-12-15 13:54:09.942241 mikro-0.3.9/mikro/api/schema.py
+-rw-r--r--   0        0        0        0 2022-11-21 13:19:21.452118 mikro-0.3.9/mikro/builders.py
+-rw-r--r--   0        0        0     4468 2022-12-08 12:30:42.620796 mikro-0.3.9/mikro/cli/main.py
+-rw-r--r--   0        0        0        0 2022-08-25 14:13:51.564206 mikro-0.3.9/mikro/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-03 16:40:05.361043 mikro-0.3.9/mikro/contrib/fakts/__init__.py
+-rw-r--r--   0        0        0     1303 2022-11-21 13:24:56.296558 mikro-0.3.9/mikro/contrib/fakts/datalayer.py
+-rw-r--r--   0        0        0     4531 2022-11-21 17:10:07.795408 mikro-0.3.9/mikro/datalayer.py
+-rw-r--r--   0        0        0      156 2022-03-21 13:01:57.991994 mikro-0.3.9/mikro/errors.py
+-rw-r--r--   0        0        0     1174 2022-11-21 13:16:43.067875 mikro-0.3.9/mikro/funcs.py
+-rw-r--r--   0        0        0       92 2022-03-21 13:01:58.083994 mikro-0.3.9/mikro/links/__init__.py
+-rw-r--r--   0        0        0     2413 2022-11-21 13:12:09.135444 mikro-0.3.9/mikro/links/datalayer.py
+-rw-r--r--   0        0        0        0 2022-05-17 11:20:06.504915 mikro-0.3.9/mikro/links/errors.py
+-rw-r--r--   0        0        0      903 2022-11-21 13:21:58.284355 mikro-0.3.9/mikro/mikro.py
+-rw-r--r--   0        0        0     1522 2022-11-21 13:25:20.364567 mikro-0.3.9/mikro/rath.py
+-rw-r--r--   0        0        0    12037 2022-12-15 13:54:02.174160 mikro-0.3.9/mikro/scalars.py
+-rw-r--r--   0        0        0     4098 2022-12-12 14:45:25.646781 mikro-0.3.9/mikro/structures.py
+-rw-r--r--   0        0        0     5750 2022-12-15 10:05:28.013204 mikro-0.3.9/mikro/traits.py
+-rw-r--r--   0        0        0      805 2022-09-26 09:28:04.741028 mikro-0.3.9/mikro/widgets.py
+-rw-r--r--   0        0        0     1241 2022-12-15 14:13:59.916979 mikro-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 mikro-0.3.9/setup.py
+-rw-r--r--   0        0        0      860 1970-01-01 00:00:00.000000 mikro-0.3.9/PKG-INFO
```

### Comparing `mikro-0.3.81/mikro/contrib/fakts/datalayer.py` & `mikro-0.3.9/mikro/contrib/fakts/datalayer.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.81/mikro/funcs.py` & `mikro-0.3.9/mikro/funcs.py`

 * *Files identical despite different names*

### Comparing `mikro-0.3.81/mikro/links/datalayer.py` & `mikro-0.3.9/mikro/links/datalayer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 
 from mikro.datalayer import DataLayer, current_datalayer
-from mikro.scalars import XArrayInput, ParquetInput, BigFile
+from mikro.scalars import XArrayInput, ParquetInput
 from rath.links.parsing import ParsingLink
-from rath.operation import Operation, opify
-import ntpath
+from rath.operation import Operation
 
 
 async def apply_recursive(func, obj, typeguard):
     if isinstance(obj, dict):  # if dict, apply to each key
         return {k: await apply_recursive(func, v, typeguard) for k, v in obj.items()}
     elif isinstance(obj, list):  # if list, apply to each element
         return await asyncio.gather(
@@ -45,15 +44,14 @@
     _lock: asyncio.Lock = False
 
     _datalayer: DataLayer = None
 
     async def aconnect(self):
         self._datalayer = current_datalayer.get()
 
-
     async def aparse(self, operation: Operation) -> Operation:
         """Parse the operation (Async)
 
         Extracts the DataFrame from the operation and uploads it to the DataLayer.
 
         Args:
             operation (Operation): The operation to parse
@@ -72,17 +70,14 @@
 
         operation.variables = await apply_recursive(
             datalayer.astore_array_input, operation.variables, XArrayInput
         )
         operation.variables = await apply_recursive(
             datalayer.astore_parquet_input, operation.variables, ParquetInput
         )
-        operation.variables = await apply_recursive(
-            datalayer.astore_bigfile, operation.variables, BigFile
-        )
 
         return operation
 
     class Config:
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
         extra = "forbid"
```

### Comparing `mikro-0.3.81/mikro/rath.py` & `mikro-0.3.9/mikro/rath.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,14 @@
     client. (This allows you to use the `mikro.rath.current` function to get the
     current client, within the context of mikro app).
     
     This is a subclass of Rath that adds some default links to convert files and array to support
     the graphql multipart request spec."""
     link: MikroLinkComposition
 
-    def _repr_html_inline_(self):
-        return f"<table><tr><td>auto_connect</td><td>{self.auto_connect}</td></tr></table>"
-
     async def __aenter__(self):
         await super().__aenter__()
         current_mikro_rath.set(self)
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await super().__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `mikro-0.3.81/mikro/scalars.py` & `mikro-0.3.9/mikro/scalars.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,109 +2,48 @@
 Custom scalars for Mikro.
 
 
 """
 
 
 import os
-from typing import Any, List, IO, Optional
+from typing import Any
 import xarray as xr
+import pyarrow.parquet as pq
 import pandas as pd
 import numpy as np
-import io
-from typing import TYPE_CHECKING
-from .utils import rechunk
-import logging
-
-if TYPE_CHECKING:
-    from mikro.datalayer import DataLayer
-
-
-class AssignationID(str):
-    """A custom scalar to represent an affine matrix."""
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Validate the input array and convert it to a xr.DataArray."""
-        return cls(v)
-
-
-try:
-    from rekuest.actors.vars import (
-        get_current_assignation_helper,
-        NotWithinAnAssignationError,
-    )
-
-    def get_current_id(cls, value) -> AssignationID:
-        try:
-            return value or get_current_assignation_helper().assignment.assignation
-        except NotWithinAnAssignationError:
-            return value
-
-except ImportError:
-
-    def get_current_id(cls, value):
-        return value
 
 
 class XArrayConversionException(Exception):
-    """An exception that is raised when a conversion to xarray fails."""
-
     pass
 
 
 MetricValue = Any
 FeatureValue = Any
 
 
-class AffineMatrix(list):
-    """A custom scalar to represent an affine matrix."""
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Validate the input array and convert it to a xr.DataArray."""
-        if isinstance(v, np.ndarray):
-            assert v.ndim == 2
-            assert v.shape[0] == v.shape[1]
-            assert v.shape == (3, 3)
-            v = v.tolist()
-
-        assert isinstance(v, list)
-        return cls(v)
-
-    def as_matrix(self):
-        return np.array(self).reshape(3, 3)
-
 
 class XArrayInput:
     """A custom scalar for wrapping of every supported array like structure on
     the mikro platform. This scalar enables validation of various array formats
     into a mikro api compliant xr.DataArray.."""
 
     def __init__(self, value: xr.DataArray) -> None:
         self.value = value
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
-    def validate(cls, v: xr.DataArray):
+    def validate(cls, v):
         """Validate the input array and convert it to a xr.DataArray."""
 
         if isinstance(v, np.ndarray):
-            dims = ["c", "t", "z", "y", "x"]
+            dims = ["c", "t", "z", "x", "y"]
             v = xr.DataArray(v, dims=dims[5 - v.ndim :])
 
         if not isinstance(v, xr.DataArray):
             raise ValueError("This needs to be a instance of xarray.DataArray")
 
         if "x" not in v.dims:
             raise ValueError("Representations must always have a 'x' Dimension")
@@ -115,58 +54,34 @@
         if "t" not in v.dims:
             v = v.expand_dims("t")
         if "c" not in v.dims:
             v = v.expand_dims("c")
         if "z" not in v.dims:
             v = v.expand_dims("z")
 
-        chunks = rechunk(
-            v.sizes, itemsize=v.data.itemsize, chunksize_in_bytes=20_000_000
-        )
+        chunks = {
+            "t": 1,
+            "x": v.sizes["x"],
+            "y": v.sizes["y"],
+            "z": 1,
+            "c": 1,
+        }
 
         v = v.chunk(
             {key: chunksize for key, chunksize in chunks.items() if key in v.dims}
         )
 
         v = v.transpose(*"ctzyx")
 
         return cls(v)
 
     def __repr__(self):
         return f"InputArray({self.value})"
 
 
-class BigFile:
-    """A custom scalar for wrapping of every supported array like structure on
-    the mikro platform. This scalar enables validation of various array formats
-    into a mikro api compliant xr.DataArray.."""
-
-    def __init__(self, value: IO) -> None:
-        self.value = value
-
-    @classmethod
-    def __get_validators__(cls):
-        yield cls.validate
-
-    @classmethod
-    def validate(cls, v):
-        """Validate the input array and convert it to a xr.DataArray."""
-
-        if isinstance(v, str):
-            v = open(v, "rb")
-
-        if not isinstance(v, io.IOBase):
-            raise ValueError("This needs to be a instance of a file")
-
-        return cls(v)
-
-    def __repr__(self):
-        return f"BigFile({self.value})"
-
-
 class ParquetInput:
     """A custom scalar for ensuring a common format to support write to the
     parquet api supported by mikro. It converts the passed value into
     a compliant format.."""
 
     def __init__(self, value: pd.DataFrame) -> None:
         self.value = value
@@ -176,14 +91,15 @@
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
+
         if not isinstance(v, pd.DataFrame):
             raise ValueError("This needs to be a instance of pandas DataFrame")
 
         return cls(v)
 
     def __repr__(self):
         return f"ParquetInput({self.value})"
@@ -203,15 +119,15 @@
         self._openstore = None
 
     def arequest(self):
         """ToDO Imepelemtn, each store needs to have a request first to the resource owner
         and then we can access the data
         """
 
-    def open(self, dl: Optional["DataLayer"] = None):
+    def open(self, dl=None):
         """Opens the store and returns the zarr store object.
 
         The store is opened on the first access and then cached for later use. This is done to avoid
         opening the store on every access.
 
 
         Args:
@@ -220,17 +136,25 @@
         Returns:
             xr.DataArray: the data array
         """
         from mikro.datalayer import current_datalayer
 
         dl = dl or current_datalayer.get()
 
-        return xr.open_zarr(store=dl.open_store(self.value), consolidated=True)["data"]
+        assert (
+            dl
+        ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
+        if self._openstore is None:
+            self._openstore = xr.open_zarr(
+                store=dl.fs.get_mapper(self.value), consolidated=True
+            )["data"]
+
+        return self._openstore
 
-    async def aopen(self, dl=None, retry=True):
+    def aopen(self, dl=None):
         """Opens the store and returns the zarr store object.
 
         The store is opened on the first access and then cached for later use. This is done to avoid
         opening the store on every access.
 
 
         Args:
@@ -239,15 +163,23 @@
         Returns:
             xr.DataArray: the data array
         """
         from mikro.datalayer import current_datalayer
 
         dl = dl or current_datalayer.get()
 
-        return xr.open_zarr(store=dl.open_store(self.value), consolidated=True)["data"]
+        assert (
+            dl
+        ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
+        if self._openstore is None:
+            self._openstore = xr.open_zarr(
+                store=dl.fs.get_mapper(self.value), consolidated=True
+            )["data"]
+
+        return self._openstore
 
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
         yield cls.validate
@@ -269,21 +201,20 @@
 class Parquet:
     """A custom scalar for ensuring an interface to the datalayer api supported by mikro. It converts the graphql value
     (a string pointed to a zarr store) into a parquet dataset and then a dataframe. This is used to access the data
     in the datalayer. The store is opened on the first access and then cached for later use. This is done to avoid
     opening the store on every access. This is done to avoid unnecessary requests to the datalayer api.
     """
 
-    def __init__(self, value: str) -> None:
+    def __init__(self, value) -> None:
         self.value = value
         self._openstore = None
 
-    def open(self, dl: Optional["DataLayer"] = None):
+    def open(self, dl=None):
         from mikro.datalayer import current_datalayer
-        import pyarrow.parquet as pq
 
         dl = dl or current_datalayer.get()
 
         assert (
             dl
         ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
         if not self._openstore:
@@ -315,36 +246,22 @@
     """
 
     __file__ = True
 
     def __init__(self, value) -> None:
         self.value = value
 
-    def download(
-        self, dl: Optional["DataLayer"] = None, filename: Optional[str] = None
-    ) -> str:
-        """Downloads the file to the current working directory.
-
-        Args:
-            dl (DataLayer, optional): The datalayer. Defaults to active datalayer.
-            filename (str, optional): The filename to save the file as. Defaults to the original filename.
-
-        Returns:
-            str: The filename of the downloaded file.
-        """
+    def download(self, dl=None):
         from mikro.datalayer import current_datalayer
         import requests
         import shutil
 
         dl = dl or current_datalayer.get()
-        assert (
-            dl
-        ), "No datalayer set. This probably happened because you never connected the datalayer. Please connect (either with async or sync) and try again."
         url = f"{dl.endpoint_url}{self.value}"
-        local_filename = filename or self.value.split("/")[-1].split("?")[0]
+        local_filename = self.value.split("/")[-1].split("?")[0]
         with requests.get(url, stream=True) as r:
             with open(local_filename, "wb") as f:
                 shutil.copyfileobj(r.raw, f)
                 return local_filename
 
     def __enter__(self):
         self.local_file = self.download()
@@ -368,48 +285,54 @@
         # exactly
         return cls(v)
 
     def __repr__(self):
         return f"File({self.value})"
 
 
+
 class ModelFile:
     """A custom scalar to enable uploading files to the datalayer
     it enables serialization of everythign
     """
 
     __file__ = True
 
     def __init__(self, value) -> None:
         self.value = value
 
+
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
 
+
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         # you could also return a string here which would mean model.post_code
         # would be a string, pydantic won't care but you could end up with some
         # confusion since the value's type won't match the type annotation
         # exactly
         if isinstance(v, str):
             return cls(open(v, "rb"))
+        
 
         return cls(v)
 
     def __repr__(self):
         return f"ModelFile({self.value})"
 
 
-class ModelData:
+
+
+class Model:
     """A custom scalar for ensuring an interface to files api supported by mikro. It converts the graphql value
     (a string pointed to a zarr store) into a downloadable file. To access the file you need to call the download
     method. This is done to avoid unnecessary requests to the datalayer api.
     """
 
     __file__ = True
 
@@ -438,14 +361,15 @@
 
     @classmethod
     def __get_validators__(cls):
         # one or more validators may be yielded which will be called in the
         # order to validate the input, each validator will receive as an input
         # the value returned from the previous validator
 
+
         yield cls.validate
 
     @classmethod
     def validate(cls, v):
         # you could also return a string here which would mean model.post_code
         # would be a string, pydantic won't care but you could end up with some
         # confusion since the value's type won't match the type annotation
```

### Comparing `mikro-0.3.81/PKG-INFO` & `mikro-0.3.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: mikro
-Version: 0.3.81
+Version: 0.3.9
 Summary: images for arkitekt
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
-Requires-Python: >=3.8,<=3.12
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: complete
-Provides-Extra: table
 Provides-Extra: turms
-Requires-Dist: dask (>=2023.3.0,<2024.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pyarrow (>=11.0) ; (python_version >= "3.8") and (extra == "table" or extra == "complete")
-Requires-Dist: rath (>=0.3.6)
-Requires-Dist: s3fs (>=2023.1.0,<2024.0.0)
-Requires-Dist: xarray (>=2022.12.0)
-Requires-Dist: zarr (>=2.14.2,<3.0.0)
+Requires-Dist: dask (>=2022.2.1,<2023.0.0)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: pyarrow (>=6.0.1,<7.0.0)
+Requires-Dist: rath (>=0.3.3)
+Requires-Dist: s3fs (>=2022.2.0,<2023.0.0)
+Requires-Dist: turms (>=0.2.3,<0.3.0); (python_version >= "3.9") and (extra == "turms" or extra == "complete")
+Requires-Dist: xarray (>=2022.3.0,<2023.0.0)
+Requires-Dist: zarr (>=2.11.1,<3.0.0)
```

