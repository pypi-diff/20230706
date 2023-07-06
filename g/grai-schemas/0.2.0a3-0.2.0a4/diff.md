# Comparing `tmp/grai_schemas-0.2.0a3.tar.gz` & `tmp/grai_schemas-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.2.0a3.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a4.tar", max compression
```

## Comparing `grai_schemas-0.2.0a3.tar` & `grai_schemas-0.2.0a4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a3/LICENSE
--rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a3/README.md
--rw-r--r--   0        0        0      834 2023-06-30 12:39:18.742499 grai_schemas-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0      210 2023-06-30 12:39:29.306536 grai_schemas-0.2.0a3/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      848 2023-06-30 08:46:34.984841 grai_schemas-0.2.0a3/src/grai_schemas/base.py
--rw-r--r--   0        0        0     3715 2023-06-29 08:12:22.804993 grai_schemas-0.2.0a3/src/grai_schemas/generics.py
--rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a3/src/grai_schemas/human_ids.py
--rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a3/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a3/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      669 2023-06-30 08:46:34.985057 grai_schemas-0.2.0a3/src/grai_schemas/schema.py
--rw-r--r--   0        0        0     2568 2023-06-16 16:15:18.436927 grai_schemas-0.2.0a3/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      440 2023-06-29 08:12:22.805122 grai_schemas-0.2.0a3/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     2786 2023-06-29 08:12:22.805233 grai_schemas-0.2.0a3/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0        0 2023-06-29 08:12:22.805263 grai_schemas-0.2.0a3/src/grai_schemas/v1/events
--rw-r--r--   0        0        0      845 2023-06-29 08:12:22.805491 grai_schemas-0.2.0a3/src/grai_schemas/v1/events.py
--rw-r--r--   0        0        0      858 2023-06-29 08:12:22.805602 grai_schemas-0.2.0a3/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     2067 2023-06-29 08:12:22.805723 grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      321 2023-06-16 16:15:18.437462 grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/generics.py
--rw-r--r--   0        0        0      779 2023-06-29 08:12:22.805839 grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     2006 2023-06-30 08:46:34.985392 grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     6925 2023-06-29 08:12:22.806053 grai_schemas-0.2.0a3/src/grai_schemas/v1/mock.py
--rw-r--r--   0        0        0     2776 2023-06-29 08:12:22.806146 grai_schemas-0.2.0a3/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0      940 2023-06-29 08:12:22.806213 grai_schemas-0.2.0a3/src/grai_schemas/v1/organization.py
--rw-r--r--   0        0        0     1325 2023-06-29 08:12:22.806285 grai_schemas-0.2.0a3/src/grai_schemas/v1/source.py
--rw-r--r--   0        0        0     3710 2023-06-30 12:27:26.107980 grai_schemas-0.2.0a3/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a4/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a4/README.md
+-rw-r--r--   0        0        0      862 2023-07-05 16:59:28.458708 grai_schemas-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-07-05 16:59:33.885947 grai_schemas-0.2.0a4/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      848 2023-06-30 08:46:34.984841 grai_schemas-0.2.0a4/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3757 2023-07-03 12:38:54.726590 grai_schemas-0.2.0a4/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a4/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a4/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a4/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      669 2023-06-30 08:46:34.985057 grai_schemas-0.2.0a4/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2564 2023-07-03 12:38:54.727678 grai_schemas-0.2.0a4/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      451 2023-07-03 12:38:54.727777 grai_schemas-0.2.0a4/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     2786 2023-06-29 08:12:22.805233 grai_schemas-0.2.0a4/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:12:22.805263 grai_schemas-0.2.0a4/src/grai_schemas/v1/events
+-rw-r--r--   0        0        0      845 2023-06-29 08:12:22.805491 grai_schemas-0.2.0a4/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      793 2023-07-03 12:38:54.727867 grai_schemas-0.2.0a4/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0     1738 2023-07-03 12:38:54.727925 grai_schemas-0.2.0a4/src/grai_schemas/v1/merge.py
+-rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2179 2023-07-03 12:38:54.728133 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      240 2023-07-03 12:38:54.728222 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0      784 2023-07-03 12:38:54.728309 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     1930 2023-07-03 12:38:54.728593 grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     6925 2023-06-29 08:12:22.806053 grai_schemas-0.2.0a4/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     2776 2023-06-29 08:12:22.806146 grai_schemas-0.2.0a4/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-06-29 08:12:22.806213 grai_schemas-0.2.0a4/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1254 2023-07-05 16:59:13.277528 grai_schemas-0.2.0a4/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3696 2023-06-30 16:06:45.947383 grai_schemas-0.2.0a4/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a4/PKG-INFO
```

### Comparing `grai_schemas-0.2.0a3/LICENSE` & `grai_schemas-0.2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/pyproject.toml` & `grai_schemas-0.2.0a4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.2.0-alpha3"
+version = "0.2.0-alpha4"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
 readme = "README.md"
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
@@ -17,14 +17,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pre-commit = "^2.21.0"
 pytest = "^7.2.0"
 mypy = "^0.991"
+pytest-durations = "^1.2.0"
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 line-length = 120
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/base.py` & `grai_schemas-0.2.0a4/src/grai_schemas/base.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/generics.py` & `grai_schemas-0.2.0a4/src/grai_schemas/generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,18 @@
     class Config:
         """ """
 
         validate_assignment = True
         validate_all = True
 
 
+class Metadata(GraiBaseModel):
+    pass
+
+
 class MalformedMetadata(GraiBaseModel):
     """ """
 
     malformed_values: Dict = {}
 
     @root_validator(pre=True)
     def validate_malformed(cls, v):
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/human_ids.py` & `grai_schemas-0.2.0a4/src/grai_schemas/human_ids.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/schema.py` & `grai_schemas-0.2.0a4/src/grai_schemas/schema.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/utilities.py` & `grai_schemas-0.2.0a4/src/grai_schemas/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,30 +76,28 @@
     Raises:
 
     """
     return a
 
 
 @merge.register
-def merge_dicts(a: dict, b: dict) -> dict:
+def merge_dict_item(a: Dict, b: Dict) -> Dict:
     """
 
     Args:
-        a (dict):
-        b (dict):
+        a (Dict):
+        b (Dict):
 
     Returns:
 
     Raises:
 
     """
-    result = {**a}
-    for k, v in b.items():
-        result[k] = merge(result[k], v) if k in result else v
-
+    result = {**a, **b}
+    result.update({key: merge(a[key], b[key]) for key in a.keys() & b.keys()})
     return result
 
 
 @merge.register
 def merge_list(a: list, b: list) -> list:
     """
 
@@ -156,15 +154,15 @@
         b (Any):
 
     Returns:
 
     Raises:
 
     """
-    merged = merge(a.dict(), b)
+    merged = merge(dict(a), b)
     return type(a)(**merged)
 
 
 @merge.register
 def merge_pydantic_right(a: T, b: BaseModel) -> T:
     """
 
@@ -173,15 +171,15 @@
         b (BaseModel):
 
     Returns:
 
     Raises:
 
     """
-    return merge(a, b.dict())
+    return merge(a, dict(b))
 
 
 def merge_models(a: T, b: T) -> T:
     """This function is deprecated. Use `merge` instead
 
     Args:
         a (T):
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/edge.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/edge.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/events.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/events.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/generics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 from typing import Literal, Optional, Union
 from uuid import UUID
 
-from grai_schemas.generics import GraiBaseModel
+from grai_schemas.generics import GraiBaseModel, Metadata
 from pydantic import BaseModel
 
 
-class V1Mixin(BaseModel):
-    """ """
-
-    version: Literal["v1"] = "v1"
-
-
 class BaseID(GraiBaseModel):
     """ """
 
     id: Optional[UUID]
     name: Optional[str]
     namespace: Optional[str]
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/edges.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/edges.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import Enum
 from typing import Any, Dict, List, Literal, Optional, Union
 
-from grai_schemas.generics import MalformedMetadata
-from grai_schemas.v1.generics import V1Mixin
+from grai_schemas.generics import GraiBaseModel, MalformedMetadata
 from grai_schemas.v1.metadata.generics import GenericAttributes
 
 
 class EdgeMetadataTypeLabels(Enum):
     """ """
 
     generic = "Generic"
@@ -14,18 +13,19 @@
     column_to_column = "ColumnToColumn"
     table_to_table = "TableToTable"
 
 
 EdgeTypeLabelLiterals = Literal["Generic", "TableToColumn", "ColumnToColumn", "TableToTable"]
 
 
-class BaseEdgeMetadataV1(V1Mixin):
+class BaseEdgeMetadataV1(GraiBaseModel):
     """ """
 
     type: Literal["EdgeV1"] = "EdgeV1"
+    version: Literal["v1"] = "v1"
     edge_type: EdgeTypeLabelLiterals
     edge_attributes: GenericAttributes
     tags: Optional[List[str]]
 
 
 class MalformedEdgeMetadataV1(MalformedMetadata, BaseEdgeMetadataV1):
     edge_type: Optional[str] = "Malformed"  # type: ignore
@@ -36,40 +36,43 @@
     edge_type: Literal["Generic"]
     edge_attributes: GenericAttributes = GenericAttributes()
 
 
 class TableToColumnAttributes(GenericAttributes):
     """ """
 
+    version: Literal["v1"] = "v1"
     pass
 
 
 class TableToColumnMetadata(BaseEdgeMetadataV1):
     """ """
 
     edge_type: Literal["TableToColumn"]
     edge_attributes: TableToColumnAttributes = TableToColumnAttributes()
 
 
 class TableToTableAttributes(GenericAttributes):
     """ """
 
+    version: Literal["v1"] = "v1"
     pass
 
 
 class TableToTableMetadata(BaseEdgeMetadataV1):
     """ """
 
     edge_type: Literal["TableToTable"]
     edge_attributes: TableToTableAttributes = TableToTableAttributes()
 
 
 class ColumnToColumnAttributes(GenericAttributes):
     """ """
 
+    version: Literal["v1"] = "v1"
     preserves_data_type: Optional[bool] = None
     preserves_nullable: Optional[bool] = None
     preserves_unique: Optional[bool] = None
 
 
 class ColumnToColumnMetadata(BaseEdgeMetadataV1):
     """ """
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/metadata.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Optional, Union
 
-from grai_schemas.generics import GraiBaseModel, MalformedMetadata
+from grai_schemas.generics import GraiBaseModel, MalformedMetadata, Metadata
 from grai_schemas.utilities import merge
 from grai_schemas.v1.metadata import edges, nodes
 
 
-class GraiMetadataV1(GraiBaseModel):
+class GraiMetadataV1(Metadata):
     """ """
 
     grai: Union[edges.Metadata, nodes.Metadata]
 
 
 class MetadataV1(GraiMetadataV1):
     """ """
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/metadata/nodes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from enum import Enum
 from typing import Any, List, Literal, Optional, Union
 
-from grai_schemas.generics import DefaultValue, HashableBaseModel, MalformedMetadata
-from grai_schemas.v1.generics import GraiBaseModel, V1Mixin
+from grai_schemas.generics import (
+    DefaultValue,
+    GraiBaseModel,
+    HashableBaseModel,
+    MalformedMetadata,
+)
 from grai_schemas.v1.metadata.generics import GenericAttributes
 
 
 class NodeMetadataTypeLabels(Enum):
     """ """
 
     generic: Literal["Generic"] = "Generic"
@@ -19,18 +23,19 @@
 
 class SourceType(Enum):
     """ """
 
     database = "SQL"
 
 
-class BaseNodeMetadataV1(V1Mixin):
+class BaseNodeMetadataV1(GraiBaseModel):
     """ """
 
     type: Literal["NodeV1"] = "NodeV1"
+    version: Literal["v1"] = "v1"
     node_type: NodeMetadataTypeLabelLiterals
     node_attributes: GenericAttributes
     tags: Optional[List[str]]
 
 
 class MalformedNodeMetadataV1(MalformedMetadata, BaseNodeMetadataV1):
     """ """
@@ -40,41 +45,39 @@
 
 
 class GenericNodeMetadataV1(BaseNodeMetadataV1):
     node_type: Literal["Generic"]
     node_attributes: GenericAttributes = GenericAttributes()
 
 
-class ColumnAttributes(V1Mixin, GenericAttributes):
+class ColumnAttributes(GenericAttributes):
     """ """
 
+    version: Literal["v1"] = "v1"
     data_type: Optional[str]  # This will need to be standardized
     default_value: Optional[DefaultValue]
     is_nullable: Optional[bool]
     is_unique: Optional[bool]
     is_primary_key: Optional[bool]
 
 
 class ColumnMetadata(BaseNodeMetadataV1):
     """ """
 
     node_type: Literal["Column"]
     node_attributes: ColumnAttributes = ColumnAttributes()
 
 
-class TableAttributes(V1Mixin, GenericAttributes):
+class TableAttributes(GenericAttributes):
     """ """
 
-    pass
+    version: Literal["v1"] = "v1"
 
 
 class TableMetadata(BaseNodeMetadataV1):
     """ """
 
     node_type: Literal["Table"]
     node_attributes: TableAttributes = TableAttributes()
 
 
-x = {"version": "v1", "node_type": NodeMetadataTypeLabels.table.value, "node_attributes": {}, "tags": ["a_tag"]}
-TableMetadata(**x)
-
 Metadata = Union[ColumnMetadata, TableMetadata, GenericNodeMetadataV1]
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/mock.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/mock.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/node.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/node.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/organization.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/organization.py`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/source.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 class SourceSpec(GraiBaseModel):
     id: Optional[UUID]
     name: str
     workspace: Union[UUID, WorkspaceSpec, None]
 
     @property
     def workspace_id(self) -> Optional[UUID]:
-        return self.workspace.id if isinstance(self.workspace, WorkspaceSpec) else self.workspace
+        return (
+            self.workspace.id
+            if isinstance(self.workspace, WorkspaceSpec)
+            else self.workspace
+        )
 
     def __hash__(self) -> int:
-        if self.workspace_id is None:
-            raise ValueError("Cannot hash a source spec without a workspace id")
         return hash(self.name)
 
 
 class DataSourceMixin(GraiBaseModel):
     data_source: SourceSpec
```

### Comparing `grai_schemas-0.2.0a3/src/grai_schemas/v1/workspace.py` & `grai_schemas-0.2.0a4/src/grai_schemas/v1/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     search_enabled: Optional[bool]
 
     @property
     def organization(self):
         return self.organisation
 
     @validator("organisation", always=True, pre=True)
-    def validate_organisation(
-        cls, v: Union[UUID, str, Dict, OrganisationSpec]
-    ) -> Union[UUID, OrganisationSpec]:
+    def validate_organisation(cls, v: Union[UUID, str, Dict, OrganisationSpec]) -> Union[UUID, OrganisationSpec]:
         if isinstance(v, (OrganisationSpec, UUID)):
             return v
         elif isinstance(v, dict):
             return OrganisationSpec(**v)
         elif isinstance(v, str):
             try:
                 uuid_val = UUID(v)
```

### Comparing `grai_schemas-0.2.0a3/PKG-INFO` & `grai_schemas-0.2.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-schemas
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

