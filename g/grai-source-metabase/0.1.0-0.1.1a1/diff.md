# Comparing `tmp/grai_source_metabase-0.1.0.tar.gz` & `tmp/grai_source_metabase-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_metabase-0.1.0.tar", max compression
+gzip compressed data, was "grai_source_metabase-0.1.1a1.tar", max compression
```

## Comparing `grai_source_metabase-0.1.0.tar` & `grai_source_metabase-0.1.1a1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       29 2023-07-06 18:33:54.210141 grai_source_metabase-0.1.0/README.md
--rw-r--r--   0        0        0      600 2023-07-06 20:21:57.622844 grai_source_metabase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 18:33:54.211964 grai_source_metabase-0.1.0/src/grai_source_metabase/__init__.py
--rw-r--r--   0        0        0    10393 2023-07-06 18:33:54.212223 grai_source_metabase-0.1.0/src/grai_source_metabase/adapters.py
--rw-r--r--   0        0        0     1694 2023-07-06 18:33:54.212504 grai_source_metabase-0.1.0/src/grai_source_metabase/base.py
--rw-r--r--   0        0        0     9969 2023-07-06 18:33:54.212723 grai_source_metabase-0.1.0/src/grai_source_metabase/loader.py
--rw-r--r--   0        0        0     3299 2023-07-06 18:33:54.212794 grai_source_metabase-0.1.0/src/grai_source_metabase/mock_tools.py
--rw-r--r--   0        0        0      783 2023-07-06 18:33:54.212995 grai_source_metabase-0.1.0/src/grai_source_metabase/models.py
--rw-r--r--   0        0        0      186 2023-07-06 18:33:54.213324 grai_source_metabase-0.1.0/src/grai_source_metabase/package_definitions.py
--rw-r--r--   0        0        0      636 1970-01-01 00:00:00.000000 grai_source_metabase-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-07-06 18:33:54.210141 grai_source_metabase-0.1.1a1/README.md
+-rw-r--r--   0        0        0      607 2023-07-06 20:41:26.464528 grai_source_metabase-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-07-06 20:41:11.975437 grai_source_metabase-0.1.1a1/src/grai_source_metabase/__init__.py
+-rw-r--r--   0        0        0    10393 2023-07-06 18:33:54.212223 grai_source_metabase-0.1.1a1/src/grai_source_metabase/adapters.py
+-rw-r--r--   0        0        0     1624 2023-07-06 20:46:24.184345 grai_source_metabase-0.1.1a1/src/grai_source_metabase/base.py
+-rw-r--r--   0        0        0     9969 2023-07-06 18:33:54.212723 grai_source_metabase-0.1.1a1/src/grai_source_metabase/loader.py
+-rw-r--r--   0        0        0     3299 2023-07-06 18:33:54.212794 grai_source_metabase-0.1.1a1/src/grai_source_metabase/mock_tools.py
+-rw-r--r--   0        0        0      783 2023-07-06 18:33:54.212995 grai_source_metabase-0.1.1a1/src/grai_source_metabase/models.py
+-rw-r--r--   0        0        0      186 2023-07-06 18:33:54.213324 grai_source_metabase-0.1.1a1/src/grai_source_metabase/package_definitions.py
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 grai_source_metabase-0.1.1a1/PKG-INFO
```

### Comparing `grai_source_metabase-0.1.0/pyproject.toml` & `grai_source_metabase-0.1.1a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-source-metabase"
-version = "0.1.0"
+version = "0.1.1-alpha1"
 description = ""
 authors = ["Elseagle <dowolebolu@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "grai_source_metabase", from = "src" },
 ]
```

### Comparing `grai_source_metabase-0.1.0/src/grai_source_metabase/adapters.py` & `grai_source_metabase-0.1.1a1/src/grai_source_metabase/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.0/src/grai_source_metabase/base.py` & `grai_source_metabase-0.1.1a1/src/grai_source_metabase/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Literal, Optional, Tuple
 
 from grai_client.endpoints.client import BaseClient
 from grai_client.update import update
 from grai_schemas.base import Node, Edge
 
-from adapters import adapt_to_client
-from loader import MetabaseConnector
+from grai_source_metabase.adapters import adapt_to_client
+from grai_source_metabase.loader import MetabaseConnector
 
 
 def get_nodes_and_edges(
     connector: MetabaseConnector, version: Literal["v1"]
 ) -> Tuple[List[Node], List[Edge]]:
     """
 
@@ -29,37 +29,37 @@
     edges = adapt_to_client(edges, version)
     return nodes, edges
 
 
 def update_server(
     client: BaseClient,
     namespaces: Optional = None,
-    default_namespace: Optional[str] = None,
+    metabase_namespace: Optional[str] = None,
     username: Optional[str] = None,
     password: Optional[str] = None,
     endpoint: Optional[str] = None,
 ):
     """
 
     Args:
-        password: Optional[str]
+        password:
         username: Optional[str]
-        client (BaseClient):
-        namespaces (Optional[NamespaceTypes], optional):  (Default value = None)
-        default_namespace (Optional[str], optional):  (Default value = None)
-        endpoint (Optional[str], optional):  (Default value = None)
+        client:
+        namespaces:  (Default value = None)
+        metabase_namespace:  (Default value = None)
+        endpoint:  (Default value = None)
 
     Returns:
 
     Raises:
 
     """
     kwargs = {
         "namespaces": namespaces,
-        "default_namespace": default_namespace,
+        "metabase_namespace": metabase_namespace,
         "username": username,
         "password": password,
         "endpoint": endpoint,
     }
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     conn = MetabaseConnector(**kwargs)
```

### Comparing `grai_source_metabase-0.1.0/src/grai_source_metabase/loader.py` & `grai_source_metabase-0.1.1a1/src/grai_source_metabase/loader.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.0/src/grai_source_metabase/mock_tools.py` & `grai_source_metabase-0.1.1a1/src/grai_source_metabase/mock_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.0/src/grai_source_metabase/models.py` & `grai_source_metabase-0.1.1a1/src/grai_source_metabase/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_metabase-0.1.0/PKG-INFO` & `grai_source_metabase-0.1.1a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-metabase
-Version: 0.1.0
+Version: 0.1.1a1
 Summary: 
 Author: Elseagle
 Author-email: dowolebolu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

