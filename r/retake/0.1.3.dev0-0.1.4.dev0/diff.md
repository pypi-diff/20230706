# Comparing `tmp/retake-0.1.3.dev0.tar.gz` & `tmp/retake-0.1.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake-0.1.3.dev0.tar", max compression
+gzip compressed data, was "retake-0.1.4.dev0.tar", max compression
```

## Comparing `retake-0.1.3.dev0.tar` & `retake-0.1.4.dev0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.3.dev0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.3.dev0/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.3.dev0/core/extract/__init__.py
--rw-r--r--   0        0        0     1494 2023-07-05 01:31:03.011534 retake-0.1.3.dev0/core/extract/postgres.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.3.dev0/core/load/__init__.py
--rw-r--r--   0        0        0     5122 2023-07-05 19:05:09.415038 retake-0.1.3.dev0/core/load/elasticsearch.py
--rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.3.dev0/core/load/opensearch.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.3.dev0/core/transform/__init__.py
--rw-r--r--   0        0        0      263 2023-07-05 01:31:03.012356 retake-0.1.3.dev0/core/transform/embedding.py
--rw-r--r--   0        0        0      472 2023-07-05 19:07:15.844253 retake-0.1.3.dev0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-05 19:05:09.416653 retake-0.1.3.dev0/retake/__init__.py
--rw-r--r--   0        0        0      235 2023-07-05 19:05:09.416833 retake-0.1.3.dev0/retake/embedding.py
--rw-r--r--   0        0        0     2067 2023-07-05 19:05:09.417132 retake-0.1.3.dev0/retake/pipeline.py
--rw-r--r--   0        0        0      662 2023-07-05 19:05:09.417415 retake-0.1.3.dev0/retake/sink.py
--rw-r--r--   0        0        0      384 2023-07-05 19:05:09.417695 retake-0.1.3.dev0/retake/source.py
--rw-r--r--   0        0        0      356 2023-07-05 19:05:09.417908 retake-0.1.3.dev0/retake/target.py
--rw-r--r--   0        0        0      752 2023-07-05 19:05:09.418073 retake-0.1.3.dev0/retake/transform.py
--rw-r--r--   0        0        0     1965 1970-01-01 00:00:00.000000 retake-0.1.3.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.4.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.4.dev0/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.4.dev0/core/extract/__init__.py
+-rw-r--r--   0        0        0      326 2023-07-05 22:15:59.015798 retake-0.1.4.dev0/core/extract/base.py
+-rw-r--r--   0        0        0     1780 2023-07-05 22:15:59.024548 retake-0.1.4.dev0/core/extract/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.4.dev0/core/load/__init__.py
+-rw-r--r--   0        0        0      575 2023-07-05 19:36:34.019152 retake-0.1.4.dev0/core/load/base.py
+-rw-r--r--   0        0        0     5200 2023-07-05 19:36:34.041171 retake-0.1.4.dev0/core/load/elasticsearch.py
+-rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.4.dev0/core/load/opensearch.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.4.dev0/core/transform/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-05 22:15:59.016190 retake-0.1.4.dev0/core/transform/base.py
+-rw-r--r--   0        0        0      646 2023-07-05 22:15:59.018406 retake-0.1.4.dev0/core/transform/embedding.py
+-rw-r--r--   0        0        0      523 2023-07-05 22:20:42.774209 retake-0.1.4.dev0/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-05 19:05:09.416653 retake-0.1.4.dev0/retake/__init__.py
+-rw-r--r--   0        0        0      594 2023-07-05 22:15:59.021471 retake-0.1.4.dev0/retake/embedding.py
+-rw-r--r--   0        0        0     3604 2023-07-05 22:15:59.039299 retake-0.1.4.dev0/retake/pipeline.py
+-rw-r--r--   0        0        0      812 2023-07-05 21:03:51.198603 retake-0.1.4.dev0/retake/sink.py
+-rw-r--r--   0        0        0      384 2023-07-05 19:05:09.417695 retake-0.1.4.dev0/retake/source.py
+-rw-r--r--   0        0        0      356 2023-07-05 19:05:09.417908 retake-0.1.4.dev0/retake/target.py
+-rw-r--r--   0        0        0      752 2023-07-05 19:05:09.418073 retake-0.1.4.dev0/retake/transform.py
+-rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 retake-0.1.4.dev0/PKG-INFO
```

### Comparing `retake-0.1.3.dev0/README.md` & `retake-0.1.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `retake-0.1.3.dev0/core/extract/postgres.py` & `retake-0.1.4.dev0/core/extract/postgres.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import select
 import json
 import threading
 import queue
 
 from psycopg2.extras import LogicalReplicationConnection
 from psycopg2.extensions import ISOLATION_LEVEL_AUTOCOMMIT
+from typing import List
+
+from core.extract.base import Extractor
 
 
 class ConnectionError(Exception):
     pass
 
 
-class PostgresExtractor:
+class PostgresExtractor(Extractor):
     def __init__(self, dsn: str):
         self.dsn = dsn
         self.connection = None
         self.cursor = None
-        self.chunk_size = 1000
 
         self._connect(dsn)
 
     def _connect(self, dsn: str):
         try:
             self.connection = psycopg2.connect(
                 self.dsn, connection_factory=LogicalReplicationConnection
@@ -29,33 +31,40 @@
         except psycopg2.ProgrammingError:
             raise ConnectionError("Unable to connect to database")
         except psycopg2.OperationalError:
             raise ConnectionError("Unable to connect to database")
 
         self.cursor = self.connection.cursor()
 
-    def disconnect(self):
+    def teardown(self):
+        self.cursor.close()
         self.connection.close()
 
-    def fetch_rows(self, table, columns):
+    def count(self, relation: str):
+        self.cursor.execute(f"SELECT COUNT(*) FROM {relation}")
+        return self.cursor.fetchone()[0]
+
+    def extract_all(
+        self, relation: str, columns: List[str], primary_key: str, chunk_size: int
+    ):
         offset = 0
         columns_str = ", ".join(columns)
 
         while True:
             self.cursor.execute(
                 f"""
                 SELECT {columns_str}
-                FROM {table}
-                ORDER BY id
+                FROM {relation}
+                ORDER BY {primary_key}
                 LIMIT %s
                 OFFSET %s
             """,
-                (self.chunk_size, offset),
+                (chunk_size, offset),
             )
 
             rows = self.cursor.fetchall()
 
             if not rows:
                 break
 
             yield rows
-            offset += self.chunk_size
+            offset += chunk_size
```

### Comparing `retake-0.1.3.dev0/core/load/elasticsearch.py` & `retake-0.1.4.dev0/core/load/elasticsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from abc import ABC, abstractmethod
 from elasticsearch import Elasticsearch, helpers
 from typing import Dict, List, Union
+from core.load.base import Loader
 
 
 class FieldTypeError(Exception):
     pass
 
 
-class ElasticSearchLoader:
+class ElasticSearchLoader(Loader):
     def __init__(
         self,
         host: str = None,
         user: str = None,
         password: str = None,
         ssl_assert_fingerprint: str = None,
         cloud_id: str = None,
```

### Comparing `retake-0.1.3.dev0/retake/transform.py` & `retake-0.1.4.dev0/retake/transform.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.3.dev0/PKG-INFO` & `retake-0.1.4.dev0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: retake
-Version: 0.1.3.dev0
+Version: 0.1.4.dev0
 Summary: Real-time pipelines for vectors
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Retake Connect
 
 ## Overview
 Retake is a real-time embeddings database with pre-built, real-time connectors to your "sources of truth" (i.e. Postgres, MySQL, etc.). This enables you to integrate embeddings with your existing databases effortlessly, ensuring that your embeddings are always up-to-date with the underlying data sources.
```

