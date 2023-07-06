# Comparing `tmp/dagster_polars-0.0.4.tar.gz` & `tmp/dagster_polars-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.4.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.5.tar", max compression
```

## Comparing `dagster_polars-0.0.4.tar` & `dagster_polars-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11344 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/LICENSE
--rw-r--r--   0        0        0     3158 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/README.md
--rw-r--r--   0        0        0      358 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/__init__.py
--rw-r--r--   0        0        0       76 2023-06-30 18:53:16.726448 dagster_polars-0.0.4/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     7896 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     7200 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/bigquery.py
--rw-r--r--   0        0        0     4417 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/delta.py
--rw-r--r--   0        0        0     2143 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0     3936 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/io_managers/utils.py
--rw-r--r--   0        0        0        0 2023-06-30 18:52:46.436453 dagster_polars-0.0.4/dagster_polars/py.typed
--rw-r--r--   0        0        0     2878 2023-06-30 18:53:16.726448 dagster_polars-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 dagster_polars-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3882 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/README.md
+-rw-r--r--   0        0        0      358 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       76 2023-07-06 11:37:09.484852 dagster_polars-0.0.5/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     5195 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     7200 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0     4593 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/delta.py
+-rw-r--r--   0        0        0     2143 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     3936 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 11:36:38.280921 dagster_polars-0.0.5/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2878 2023-07-06 11:37:09.484852 dagster_polars-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 dagster_polars-0.0.5/PKG-INFO
```

### Comparing `dagster_polars-0.0.4/LICENSE` & `dagster_polars-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.4/README.md` & `dagster_polars-0.0.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,37 +24,60 @@
 
 To use the `BigQueryPolarsIOManager` you need to install the `gcp` extra:
 ```shell
 pip install 'dagster-polars[gcp]'
 ```
 
 
-### Usage
+### Usage & Examples
 ```python
 import polars as pl
-from dagster import asset, Definitions
-from dagster_polars import PolarsParquetIOManager
+from dagster import AssetIn, Definitions, asset
+from dagster_polars import PolarsDeltaIOManager, PolarsParquetIOManager
 
 
 @asset(io_manager_key="polars_parquet_io_manager")
 def upstream() -> pl.DataFrame:
-    df: pl.DataFrame = ...
-    return df
+    return pl.DataFrame({"a": [1, 2, 3], "b": ["a", "b", "c"]})
 
 
-@asset(io_manager_key="polars_parquet_io_manager")
-def downstream(upstream: pl.LazyFrame) -> pl.DataFrame:
+@asset(
+    io_manager_key="polars_parquet_io_manager",
+    ins={"upstream": AssetIn(metadata={"columns": ["a"]})}  # explicitly specify which columns to load
+)
+def downstream(
+    upstream: pl.LazyFrame  # the type annotation controls whether we load an eager or lazy DataFrame
+) -> pl.DataFrame:
     df = ...  # some lazy operations with `upstream`
     return df.collect()
 
 
+@asset(
+    io_manager_key="polars_delta_io_manager",
+    metadata={
+        "mode": "append"  # append to the existing table instead of overwriting it
+    }
+)
+def downstream_append(
+    upstream: pl.DataFrame
+) -> pl.DataFrame:
+    return upstream
+
+
+base_dir = "/remote/or/local/path"  # s3://my-bucket/... or gs://my-bucket/... also works!
+
 definitions = Definitions(
-    assets=[upstream, downstream],
+    assets=[upstream, downstream, downstream_append],
     resources={
-        "polars_parquet_io_manager": PolarsParquetIOManager(base_dir="/remote/or/local/path")
+        "polars_parquet_io_manager": PolarsParquetIOManager(
+            base_dir=base_dir
+        ),
+        "polars_delta_io_manager": PolarsDeltaIOManager(
+            base_dir=base_dir
+        ),
     }
 )
 ```
 
 ## Development
 
 ### Installation
```

### Comparing `dagster_polars-0.0.4/dagster_polars/io_managers/bigquery.py` & `dagster_polars-0.0.5/dagster_polars/io_managers/bigquery.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.4/dagster_polars/io_managers/delta.py` & `dagster_polars-0.0.5/dagster_polars/io_managers/delta.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,27 +81,30 @@
 
         if context.has_asset_partitions:
             partition_by = context.metadata.get("partition_by")
             if partition_by is not None:
                 metadata["partition_by"] = partition_by
 
         if context.metadata.get("mode") == "append":
-            # FIXME: what to do if we are appending to a partitioned table?
-            # we should not be using the full table length,
-            # but it's unclear how to get the length of the partition we are appending to
+            # modify the medatata to reflect the fact that we are appending to the table
 
             if context.has_asset_partitions:
-                paths = self._get_paths_for_partitions(context)
-                assert len(paths) == 1
-                path = list(paths.values())[0]
+                # paths = self._get_paths_for_partitions(context)
+                # assert len(paths) == 1
+                # path = list(paths.values())[0]
+
+                # FIXME: what to about row_count metadata do if we are appending to a partitioned table?
+                # we should not be using the full table length,
+                # but it's unclear how to get the length of the partition we are appending to
+                pass
             else:
-                path = self._get_path(context)
+                metadata["append_row_count"] = metadata["row_count"]
 
-            if not context.has_asset_partitions:
-                # we need to get num_rows from the full table
-                metadata["num_rows"] = MetadataValue.int(
+                path = self._get_path(context)
+                # we need to get row_count from the full table
+                metadata["row_count"] = MetadataValue.int(
                     DeltaTable(str(path), storage_options=self.get_storage_options(path))
                     .to_pyarrow_dataset()
                     .count_rows()
                 )
 
         return metadata
```

### Comparing `dagster_polars-0.0.4/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.0.5/dagster_polars/io_managers/parquet.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.4/dagster_polars/io_managers/utils.py` & `dagster_polars-0.0.5/dagster_polars/io_managers/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.4/pyproject.toml` & `dagster_polars-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.4"
+version = "0.0.5"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
```

### Comparing `dagster_polars-0.0.4/PKG-INFO` & `dagster_polars-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -56,37 +56,60 @@
 
 To use the `BigQueryPolarsIOManager` you need to install the `gcp` extra:
 ```shell
 pip install 'dagster-polars[gcp]'
 ```
 
 
-### Usage
+### Usage & Examples
 ```python
 import polars as pl
-from dagster import asset, Definitions
-from dagster_polars import PolarsParquetIOManager
+from dagster import AssetIn, Definitions, asset
+from dagster_polars import PolarsDeltaIOManager, PolarsParquetIOManager
 
 
 @asset(io_manager_key="polars_parquet_io_manager")
 def upstream() -> pl.DataFrame:
-    df: pl.DataFrame = ...
-    return df
+    return pl.DataFrame({"a": [1, 2, 3], "b": ["a", "b", "c"]})
 
 
-@asset(io_manager_key="polars_parquet_io_manager")
-def downstream(upstream: pl.LazyFrame) -> pl.DataFrame:
+@asset(
+    io_manager_key="polars_parquet_io_manager",
+    ins={"upstream": AssetIn(metadata={"columns": ["a"]})}  # explicitly specify which columns to load
+)
+def downstream(
+    upstream: pl.LazyFrame  # the type annotation controls whether we load an eager or lazy DataFrame
+) -> pl.DataFrame:
     df = ...  # some lazy operations with `upstream`
     return df.collect()
 
 
+@asset(
+    io_manager_key="polars_delta_io_manager",
+    metadata={
+        "mode": "append"  # append to the existing table instead of overwriting it
+    }
+)
+def downstream_append(
+    upstream: pl.DataFrame
+) -> pl.DataFrame:
+    return upstream
+
+
+base_dir = "/remote/or/local/path"  # s3://my-bucket/... or gs://my-bucket/... also works!
+
 definitions = Definitions(
-    assets=[upstream, downstream],
+    assets=[upstream, downstream, downstream_append],
     resources={
-        "polars_parquet_io_manager": PolarsParquetIOManager(base_dir="/remote/or/local/path")
+        "polars_parquet_io_manager": PolarsParquetIOManager(
+            base_dir=base_dir
+        ),
+        "polars_delta_io_manager": PolarsDeltaIOManager(
+            base_dir=base_dir
+        ),
     }
 )
 ```
 
 ## Development
 
 ### Installation
```

