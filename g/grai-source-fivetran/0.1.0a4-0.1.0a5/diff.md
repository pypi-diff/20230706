# Comparing `tmp/grai_source_fivetran-0.1.0a4.tar.gz` & `tmp/grai_source_fivetran-0.1.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_fivetran-0.1.0a4.tar", max compression
+gzip compressed data, was "grai_source_fivetran-0.1.0a5.tar", max compression
```

## Comparing `grai_source_fivetran-0.1.0a4.tar` & `grai_source_fivetran-0.1.0a5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      420 2023-05-30 08:16:23.842412 grai_source_fivetran-0.1.0a4/README.md
--rw-r--r--   0        0        0     1178 2023-07-03 12:54:00.828412 grai_source_fivetran-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0      149 2023-07-03 12:54:04.685762 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/__init__.py
--rw-r--r--   0        0        0     9094 2023-06-29 12:38:00.323844 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/adapters.py
--rw-r--r--   0        0        0     2417 2023-06-30 17:13:40.674956 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/base.py
--rw-r--r--   0        0        0        0 2023-02-17 18:10:50.922218 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/__init__.py
--rw-r--r--   0        0        0   451222 2023-06-06 17:35:16.808504 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/api_models.py
--rw-r--r--   0        0        0    69211 2023-06-06 17:35:16.809499 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/main.py
--rw-r--r--   0        0        0    16866 2023-06-06 17:35:16.809718 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/loader.py
--rw-r--r--   0        0        0     2173 2023-06-06 17:35:16.809859 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/mock_tools.py
--rw-r--r--   0        0        0     5452 2023-06-06 17:35:16.809979 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/models.py
--rw-r--r--   0        0        0      199 2023-06-06 17:35:16.810077 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-17 18:10:50.924423 grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/py.typed
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0      420 2023-05-30 08:16:23.842412 grai_source_fivetran-0.1.0a5/README.md
+-rw-r--r--   0        0        0     1178 2023-07-06 09:26:32.110948 grai_source_fivetran-0.1.0a5/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-07-06 09:26:59.661765 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/__init__.py
+-rw-r--r--   0        0        0     9006 2023-07-06 08:19:52.348308 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/adapters.py
+-rw-r--r--   0        0        0     2402 2023-07-06 08:19:52.348811 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/base.py
+-rw-r--r--   0        0        0        0 2023-02-17 18:10:50.922218 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/__init__.py
+-rw-r--r--   0        0        0   451222 2023-06-06 17:35:16.808504 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/api_models.py
+-rw-r--r--   0        0        0    69211 2023-06-06 17:35:16.809499 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/main.py
+-rw-r--r--   0        0        0    16682 2023-07-06 08:19:52.349407 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/loader.py
+-rw-r--r--   0        0        0     2173 2023-06-06 17:35:16.809859 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/mock_tools.py
+-rw-r--r--   0        0        0     5452 2023-06-06 17:35:16.809979 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/models.py
+-rw-r--r--   0        0        0      199 2023-06-06 17:35:16.810077 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-17 18:10:50.924423 grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/py.typed
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 grai_source_fivetran-0.1.0a5/PKG-INFO
```

### Comparing `grai_source_fivetran-0.1.0a4/pyproject.toml` & `grai_source_fivetran-0.1.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_fivetran"
-version = "0.1.0-alpha4"
+version = "0.1.0-alpha5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_fivetran", from = "src" },
 ]
 readme = "README.md"
@@ -12,15 +12,15 @@
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran"
 documentation = "https://docs.grai.io/"
 
 
 [tool.poetry.dependencies]
 python = "^3.9.13"
 pydantic = "^1.9.1"
-grai-client = {version = "^0.3.0a10", allow-prereleases = true}
+grai-client = {version = "^0.3.0a19", allow-prereleases = true}
 grai-schemas = {version = "^0.2.0a1", allow-prereleases = true}
 multimethod = "^1.8"
 fivetran = "^0.7.0"
 requests = "^2.28.1"
 python-dotenv = "^0.21.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/adapters.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,16 +256,17 @@
 
 
 @adapt_to_client.register
 def adapt_column_to_client(current: Column, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Column):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -279,16 +280,17 @@
 
 
 @adapt_to_client.register
 def adapt_table_to_client(current: Table, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
-        current (Table):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -319,16 +321,17 @@
 
 
 @adapt_to_client.register
 def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"]) -> SourcedEdgeV1:
     """
 
     Args:
-        current (Edge):
-        version (Literal["v1"], optional):  (Default value = "v1")
+        current:
+        source:
+        version:  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
@@ -351,16 +354,16 @@
 @adapt_to_client.register
 def adapt_seq_to_client(
     objs: Sequence, source: SourceSpec, version: Literal["v1"]
 ) -> List[Union[SourcedNodeV1, SourcedEdgeV1]]:
     """
 
     Args:
-        objs (Sequence):
-        version (Literal["v1"]):
+        objs:
+        version:
 
     Returns:
 
     Raises:
 
     """
     return [adapt_to_client(item, source, version) for item in objs]
@@ -369,16 +372,17 @@
 @adapt_to_client.register
 def adapt_list_to_client(
     objs: List, source: SourceSpec, version: Literal["v1"]
 ) -> List[Union[SourcedNodeV1, SourcedEdgeV1]]:
     """
 
     Args:
-        objs (List):
-        version (Literal["v1"]):
+        objs:
+        source:
+        version:
 
     Returns:
 
     Raises:
 
     """
     return [adapt_to_client(item, source, version) for item in objs]
```

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/base.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,21 +44,21 @@
             edges (List[Edge]):
 
         Returns:
 
         Raises:
 
         """
-        node_hashes = [hash(node) for node in nodes]
-        if (n_hashes := len(set(node_hashes))) == len(nodes):
+        node_hashes = {hash(node) for node in nodes}
+        if (n_hashes := len(node_hashes)) != len(nodes):
             message = (
                 f"The Fivetran connection generated {len(nodes) - n_hashes} duplicated nodes. "
                 f"This is likely because there are multiple Fivetran tables with the same name. "
                 f"You can disambiguate these tables by identifying them with different namespaces. Please "
-                f"see the documentation for more information. https://docs.grai.io/tooling/github-actions#fivetran"
+                f"see the documentation for more information. https://docs.grai.io/integrations/fivetran"
             )
             raise ValueError(message)
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         nodes, edges = self.connector.get_nodes_and_edges()
 
         nodes = adapt_to_client(nodes, self.source, self.version)
```

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/api_models.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/fivetran_api/main.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/fivetran_api/main.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/loader.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,18 +121,18 @@
         headers: Optional[Dict] = None,
         params: Optional[Dict] = None,
         **kwargs,
     ) -> Dict:
         """
 
         Args:
-            request (Callable[..., requests.Response]):
-            url (str):
-            headers (Optional[Dict], optional):  (Default value = None)
-            params (Optional[Dict], optional):  (Default value = None)
+            request:
+            url:
+            headers:  (Default value = None)
+            params:  (Default value = None)
             **kwargs:
 
         Returns:
 
         Raises:
 
         """
@@ -149,31 +149,31 @@
         headers: Optional[Dict] = None,
         params: Optional[Dict] = None,
         **kwargs,
     ) -> Iterable[Dict]:
         """
 
         Args:
-            request (Callable[..., requests.Response]):
-            url (str):
-            headers (Optional[Dict], optional):  (Default value = None)
-            params (Optional[Dict], optional):  (Default value = None)
+            request:
+            url:
+            headers:  (Default value = None)
+            params:  (Default value = None)
             **kwargs:
 
         Returns:
 
         Raises:
 
         """
 
         def has_cursor(item: Dict) -> bool:
             """
 
             Args:
-                item (Dict):
+                item):
 
             Returns:
 
             Raises:
 
             """
             if item.get("data", {}).get("nextCursor", None) is not None:
@@ -193,17 +193,17 @@
         url: str,
         headers: Optional[Dict] = None,
         params: Optional[Dict] = None,
     ) -> List[Dict]:
         """
 
         Args:
-            url (str):
-            headers (Optional[Dict], optional):  (Default value = None)
-            params (Optional[Dict], optional):  (Default value = None)
+            url:
+            headers:  (Default value = None)
+            params:  (Default value = None)
 
         Returns:
 
         Raises:
 
         """
         query = self.paginated_query(self.session.get, url, params=params, headers=headers)
@@ -211,75 +211,75 @@
         results = [item for items in data for item in items]
         return results
 
     def get_tables(self, connector_id: str, limit: Optional[int] = None) -> List[TableMetadataResponse]:
         """
 
         Args:
-            connector_id (str):
-            limit (Optional[int], optional):  (Default value = None)
+            connector_id:
+            limit:  (Default value = None)
 
         Returns:
 
         Raises:
 
         """
         url = f"{self.config.endpoint}/metadata/connectors/{connector_id}/tables"
         return [TableMetadataResponse(**item) for item in self.get_paginated_data_items(url)]
 
     def get_columns(self, connector_id: str, limit: Optional[int] = None) -> List[ColumnMetadataResponse]:
         """
 
         Args:
-            connector_id (str):
-            limit (Optional[int], optional):  (Default value = None)
+            connector_id:
+            limit:  (Default value = None)
 
         Returns:
 
         Raises:
 
         """
         url = f"{self.config.endpoint}/metadata/connectors/{connector_id}/columns"
         return [ColumnMetadataResponse(**item) for item in self.get_paginated_data_items(url)]
 
     def get_schemas(self, connector_id: str, limit: Optional[int] = None) -> List[SchemaMetadataResponse]:
         """
 
         Args:
-            connector_id (str):
-            limit (Optional[int], optional):  (Default value = None)
+            connector_id:
+            limit:  (Default value = None)
 
         Returns:
 
         Raises:
 
         """
         url = f"{self.config.endpoint}/metadata/connectors/{connector_id}/schemas"
         return [SchemaMetadataResponse(**item) for item in self.get_paginated_data_items(url)]
 
     def get_all_groups(self, limit: Optional[int] = None) -> List[GroupResponse]:
         """
 
         Args:
-            limit (Optional[int], optional):  (Default value = None)
+            limit:  (Default value = None)
 
         Returns:
 
         Raises:
 
         """
         url = f"{self.config.endpoint}/groups"
         return [GroupResponse(**item) for item in self.get_paginated_data_items(url)]
 
     def get_group_connectors(self, group_id: str, limit: Optional[int] = None) -> List[ConnectorResponse]:
         """
 
         Args:
-            group_id (str):
-            limit (Optional[int], optional):  (Default value = None)
+            group_id:
+            limit:  (Default value = None)
 
         Returns:
 
         Raises:
 
         """
         url = f"{self.config.endpoint}/groups/{group_id}/connectors"
@@ -513,14 +513,18 @@
 
         self.table_to_conn_map: Dict[str, str] = {}
         self.column_to_conn_map: Dict[str, str] = {}
         self.schemas: Dict[str, SchemaMetadataResponse] = {}
         self.tables: Dict[str, TableMetadataResponse] = {}
         self.columns: Dict[str, ColumnMetadataResponse] = {}
 
+        self._nodes = None
+        self._edges = None
+        self.lineage_ready = False
+
     def build_lineage(self):
         """ """
         connector_ids = [[conn_id] for conn_id in self.connectors.keys()]
         schemas = self.http_runner(self.get_schemas, arg_list=connector_ids)
         tables = self.http_runner(self.get_tables, arg_list=connector_ids)
         columns = self.http_runner(self.get_columns, arg_list=connector_ids)
 
@@ -540,17 +544,21 @@
         Args:
 
         Returns:
 
         Raises:
 
         """
+        if self.lineage_ready:
+            return self._nodes, self._edges
+
+        self.build_lineage()
+
         # table.parent_id -> schema.id
         # column.parent_id -> table.id
-        self.build_lineage()
         tables = {
             table.id: Table.from_fivetran_models(
                 self.schemas[table.parent_id],
                 table,
                 self.namespace_map[self.table_to_conn_map[table.id]],
             )
             for table in self.tables.values()
@@ -569,10 +577,12 @@
         table_edges = (Edge(source=t1, destination=t2, constraint_type="c") for t1, t2 in tables.values())
         table_to_column_edges = (
             Edge(source=table, destination=col, constraint_type="bt")
             for cols in columns
             for col, table in zip(cols, tables[cols[0].fivetran_table_id])
         )
 
-        nodes = chain(chain.from_iterable(tables.values()), *columns)
-        edges = chain(column_edges, table_edges, table_to_column_edges)
-        return list(nodes), list(edges)
+        self._nodes = list(chain(chain.from_iterable(tables.values()), *columns))
+        self._edges = list(chain(column_edges, table_edges, table_to_column_edges))
+        self.lineage_ready = True
+
+        return self._nodes, self._edges
```

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/mock_tools.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a4/src/grai_source_fivetran/models.py` & `grai_source_fivetran-0.1.0a5/src/grai_source_fivetran/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_fivetran-0.1.0a4/PKG-INFO` & `grai_source_fivetran-0.1.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: grai-source-fivetran
-Version: 0.1.0a4
+Version: 0.1.0a5
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fivetran (>=0.7.0,<0.8.0)
-Requires-Dist: grai-client (>=0.3.0a10,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0a19,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
 Requires-Dist: multimethod (>=1.8,<2.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-fivetran
```

