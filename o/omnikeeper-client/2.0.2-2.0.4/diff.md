# Comparing `tmp/omnikeeper_client-2.0.2-py3-none-any.whl.zip` & `tmp/omnikeeper_client-2.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9801 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-11 15:41 omnikeeper_client/__init__.py
--rw-r--r--  2.0 unx     6718 b- defN 22-Nov-21 11:15 omnikeeper_client/functions.py
--rw-r--r--  2.0 unx      413 b- defN 22-Nov-21 10:44 omnikeeper_client/healthcheck.py
--rw-r--r--  2.0 unx     3666 b- defN 22-Nov-21 13:20 omnikeeper_client/ingest.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-13 07:44 omnikeeper_client-2.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1133 b- defN 23-Feb-13 07:44 omnikeeper_client-2.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-13 07:44 omnikeeper_client-2.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Feb-13 07:44 omnikeeper_client-2.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      779 b- defN 23-Feb-13 07:44 omnikeeper_client-2.0.2.dist-info/RECORD
-9 files, 24176 bytes uncompressed, 8441 bytes compressed:  65.1%
+Zip file size: 9596 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-06 12:16 omnikeeper_client/__init__.py
+-rw-r--r--  2.0 unx     6750 b- defN 23-Jul-06 12:16 omnikeeper_client/functions.py
+-rw-r--r--  2.0 unx      413 b- defN 23-Jul-06 12:16 omnikeeper_client/healthcheck.py
+-rw-r--r--  2.0 unx     3666 b- defN 23-Jul-06 12:16 omnikeeper_client/ingest.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 12:20 omnikeeper_client-2.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      513 b- defN 23-Jul-06 12:20 omnikeeper_client-2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 12:20 omnikeeper_client-2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-06 12:20 omnikeeper_client-2.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      778 b- defN 23-Jul-06 12:20 omnikeeper_client-2.0.4.dist-info/RECORD
+9 files, 23587 bytes uncompressed, 8236 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: omnikeeper_client/healthcheck.py
 Comment: 
 
 Filename: omnikeeper_client/ingest.py
 Comment: 
 
-Filename: omnikeeper_client-2.0.2.dist-info/LICENSE
+Filename: omnikeeper_client-2.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: omnikeeper_client-2.0.2.dist-info/METADATA
+Filename: omnikeeper_client-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: omnikeeper_client-2.0.2.dist-info/WHEEL
+Filename: omnikeeper_client-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: omnikeeper_client-2.0.2.dist-info/top_level.txt
+Filename: omnikeeper_client-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: omnikeeper_client-2.0.2.dist-info/RECORD
+Filename: omnikeeper_client-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## omnikeeper_client/functions.py

```diff
@@ -1,22 +1,26 @@
+from __future__ import annotations
+
 from oauthlib.oauth2 import LegacyApplicationClient
 from requests_oauthlib import OAuth2Session
 from gql import gql, Client
 from graphql import DocumentNode
 from gql.transport.aiohttp import AIOHTTPTransport
 import urllib.request, json
 from webcolors import hex_to_rgb
 import json
 import uuid
 from pythonjsonlogger import jsonlogger
 import logging
+
 from typing import (
     Any,
     Dict,
-    Optional,
+    Optional, Union,
+    List
 )
 
 def create_logger(level: int):
     logger = logging.getLogger()
     logger.setLevel(level)
 
     # clean up existing stuff
@@ -47,15 +51,15 @@
     return token["access_token"]
 
 def create_graphql_client(url: str, access_token: str) -> Client:
     transport = AIOHTTPTransport(url=url, headers={'Authorization': "Bearer %s" % access_token})
     client = Client(transport=transport, fetch_schema_from_transport=True)
     return client
 
-def execute_graphql(client: Client, query: str | DocumentNode, variables: Optional[Dict[str, Any]] = None):
+def execute_graphql(client: Client, query: Union[str, DocumentNode], variables: Optional[Dict[str, Any]] = None):
     prepared_query = gql(query) if query is str else query
     data = client.execute(prepared_query, variable_values=variables)
     return data
 
 def create_layer(client: Client, layer_id: str) -> bool:
     query = gql("""
     mutation ($id: String!) {
@@ -91,27 +95,26 @@
     execute_graphql(client, query, variables=dict(id=layer_id, description=description, color=argbColor))
     return True
 
 def graphQL_merged_attribute_value_to_simple_value(attribute_value: Dict[str, Any]) -> Any:
     isArray = attribute_value['isArray']
     type = attribute_value['type']
     values = attribute_value['values']
-    match type:
-        case "TEXT" | "MULTILINE_TEXT":
-            return values if isArray else values[0]
-        case "INTEGER":
-            return [int(v) for v in values] if isArray else int(values[0]) # python 3's int is 64 bit, like omnikeeper's Integer
-        case "DOUBLE":
-            return [float(v) for v in values] if isArray else float(values[0]) # python 3's float is 64 bit, like omnikeeper's Double
-        case "BOOLEAN":
-            return [bool(v) for v in values] if isArray else bool(values[0])
-        case "JSON":
-            return [json.loads(v) for v in values] if isArray else json.loads(values[0])
-        case _:
-            return values if isArray else values[0]
+    if type in ("TEXT", "MULTILINE_TEXT"):
+        return values if isArray else values[0]
+    elif type == "INTEGER":
+        return [int(v) for v in values] if isArray else int(values[0]) # python 3's int is 64 bit, like omnikeeper's Integer
+    elif type == "DOUBLE":
+        return [float(v) for v in values] if isArray else float(values[0]) # python 3's float is 64 bit, like omnikeeper's Double
+    elif type == "BOOLEAN":
+        return [bool(v) for v in values] if isArray else bool(values[0])
+    elif type == "JSON":
+        return [json.loads(v) for v in values] if isArray else json.loads(values[0])
+    else:
+        return values if isArray else values[0]
 
 def graphQL_merged_attributes_to_simple_attributes(merged_attributes: list[Dict[str, Any]]) -> Dict[str, Any]:
     return {inner['attribute']['name']: graphQL_merged_attribute_value_to_simple_value(inner['attribute']['value']) for inner in merged_attributes}
 
 def get_ci_attributes(client: Client, layer_ids: list[str], ciids: Optional[list[uuid.UUID]] = None) -> Dict[uuid.UUID, Any]:
     query = gql("""
     query ($layers: [String]!, $ciids: [Guid]) {
```

## Comparing `omnikeeper_client-2.0.2.dist-info/LICENSE` & `omnikeeper_client-2.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `omnikeeper_client-2.0.2.dist-info/RECORD` & `omnikeeper_client-2.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 omnikeeper_client/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-omnikeeper_client/functions.py,sha256=y8qaXQzyHnVFaFI9CNVfDEV1L7-2sH51p9W1ltimPc0,6718
+omnikeeper_client/functions.py,sha256=jG8oIGerazup0TTSx0RN8tZsrjVPnw2A4U0ucj768es,6750
 omnikeeper_client/healthcheck.py,sha256=jth8GYJdXVGEtr9BmXv5PUu8w6u3ToVXC-cpDmbs8uU,413
 omnikeeper_client/ingest.py,sha256=qYvOf-AQ7nIv8H5yS130Ws4JSrgenGXpgVydhiGOuOE,3666
-omnikeeper_client-2.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-omnikeeper_client-2.0.2.dist-info/METADATA,sha256=b3-c1OsNNkjHLk5vj4zUQ2IOe3k-5y_h2mJKLlU6Lcg,1133
-omnikeeper_client-2.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-omnikeeper_client-2.0.2.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
-omnikeeper_client-2.0.2.dist-info/RECORD,,
+omnikeeper_client-2.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+omnikeeper_client-2.0.4.dist-info/METADATA,sha256=Nh-LSojZF8wx9yoZdYGH_xoI3LrLmsJDmQbH23J5SS8,513
+omnikeeper_client-2.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+omnikeeper_client-2.0.4.dist-info/top_level.txt,sha256=3VgpRS-e1mbaX1mKkPt9Mszwazf6tc1Tk3GORBV6ijk,18
+omnikeeper_client-2.0.4.dist-info/RECORD,,
```

