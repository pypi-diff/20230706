# Comparing `tmp/retake-0.1.4.dev0.tar.gz` & `tmp/retake-0.1.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retake-0.1.4.dev0.tar", max compression
+gzip compressed data, was "retake-0.1.5.dev0.tar", max compression
```

## Comparing `retake-0.1.4.dev0.tar` & `retake-0.1.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.4.dev0/README.md
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.4.dev0/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.4.dev0/core/extract/__init__.py
--rw-r--r--   0        0        0      326 2023-07-05 22:15:59.015798 retake-0.1.4.dev0/core/extract/base.py
--rw-r--r--   0        0        0     1780 2023-07-05 22:15:59.024548 retake-0.1.4.dev0/core/extract/postgres.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.4.dev0/core/load/__init__.py
--rw-r--r--   0        0        0      575 2023-07-05 19:36:34.019152 retake-0.1.4.dev0/core/load/base.py
--rw-r--r--   0        0        0     5200 2023-07-05 19:36:34.041171 retake-0.1.4.dev0/core/load/elasticsearch.py
--rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.4.dev0/core/load/opensearch.py
--rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.4.dev0/core/transform/__init__.py
--rw-r--r--   0        0        0      171 2023-07-05 22:15:59.016190 retake-0.1.4.dev0/core/transform/base.py
--rw-r--r--   0        0        0      646 2023-07-05 22:15:59.018406 retake-0.1.4.dev0/core/transform/embedding.py
--rw-r--r--   0        0        0      523 2023-07-05 22:20:42.774209 retake-0.1.4.dev0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-05 19:05:09.416653 retake-0.1.4.dev0/retake/__init__.py
--rw-r--r--   0        0        0      594 2023-07-05 22:15:59.021471 retake-0.1.4.dev0/retake/embedding.py
--rw-r--r--   0        0        0     3604 2023-07-05 22:15:59.039299 retake-0.1.4.dev0/retake/pipeline.py
--rw-r--r--   0        0        0      812 2023-07-05 21:03:51.198603 retake-0.1.4.dev0/retake/sink.py
--rw-r--r--   0        0        0      384 2023-07-05 19:05:09.417695 retake-0.1.4.dev0/retake/source.py
--rw-r--r--   0        0        0      356 2023-07-05 19:05:09.417908 retake-0.1.4.dev0/retake/target.py
--rw-r--r--   0        0        0      752 2023-07-05 19:05:09.418073 retake-0.1.4.dev0/retake/transform.py
--rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 retake-0.1.4.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1454 2023-07-05 01:31:03.009679 retake-0.1.5.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011094 retake-0.1.5.dev0/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011248 retake-0.1.5.dev0/core/extract/__init__.py
+-rw-r--r--   0        0        0      326 2023-07-05 22:15:59.015798 retake-0.1.5.dev0/core/extract/base.py
+-rw-r--r--   0        0        0     2025 2023-07-05 22:50:15.971238 retake-0.1.5.dev0/core/extract/postgres.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.011590 retake-0.1.5.dev0/core/load/__init__.py
+-rw-r--r--   0        0        0      575 2023-07-05 19:36:34.019152 retake-0.1.5.dev0/core/load/base.py
+-rw-r--r--   0        0        0     5521 2023-07-06 00:00:41.649071 retake-0.1.5.dev0/core/load/elasticsearch.py
+-rw-r--r--   0        0        0      225 2023-07-05 01:31:03.012046 retake-0.1.5.dev0/core/load/opensearch.py
+-rw-r--r--   0        0        0        0 2023-07-05 01:31:03.012095 retake-0.1.5.dev0/core/transform/__init__.py
+-rw-r--r--   0        0        0      171 2023-07-05 22:15:59.016190 retake-0.1.5.dev0/core/transform/base.py
+-rw-r--r--   0        0        0      646 2023-07-05 22:15:59.018406 retake-0.1.5.dev0/core/transform/embedding.py
+-rw-r--r--   0        0        0      523 2023-07-06 00:01:58.383776 retake-0.1.5.dev0/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-07-05 19:05:09.416653 retake-0.1.5.dev0/retake/__init__.py
+-rw-r--r--   0        0        0      594 2023-07-05 22:15:59.021471 retake-0.1.5.dev0/retake/embedding.py
+-rw-r--r--   0        0        0     4031 2023-07-05 23:16:55.173185 retake-0.1.5.dev0/retake/pipeline.py
+-rw-r--r--   0        0        0      812 2023-07-05 21:03:51.198603 retake-0.1.5.dev0/retake/sink.py
+-rw-r--r--   0        0        0      384 2023-07-05 19:05:09.417695 retake-0.1.5.dev0/retake/source.py
+-rw-r--r--   0        0        0      676 2023-07-05 23:50:04.211551 retake-0.1.5.dev0/retake/target.py
+-rw-r--r--   0        0        0      752 2023-07-05 19:05:09.418073 retake-0.1.5.dev0/retake/transform.py
+-rw-r--r--   0        0        0     2057 1970-01-01 00:00:00.000000 retake-0.1.5.dev0/PKG-INFO
```

### Comparing `retake-0.1.4.dev0/README.md` & `retake-0.1.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `retake-0.1.4.dev0/core/load/base.py` & `retake-0.1.5.dev0/core/load/base.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.4.dev0/core/load/elasticsearch.py` & `retake-0.1.5.dev0/core/load/elasticsearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,57 +12,65 @@
     def __init__(
         self,
         host: str = None,
         user: str = None,
         password: str = None,
         ssl_assert_fingerprint: str = None,
         cloud_id: str = None,
+        index: bool = False,
+        similarity: str = None
     ):
+        if index and similarity is None:
+            raise ValueError("Similarity must be provided if index is True")
+
         kwargs = {
             "hosts": [host] if host else None,
             "basic_auth": (user, password) if user and password else None,
             "ssl_assert_fingerprint": ssl_assert_fingerprint
             if ssl_assert_fingerprint
             else None,
             "verify_certs": True if host else None,
             "cloud_id": cloud_id if cloud_id else None,
         }
 
         self.es = Elasticsearch(**{k: v for k, v in kwargs.items() if v is not None})
+        self.index = index
+        self.similarity = similarity
 
     ### Private Methods ###
 
     def _check_index_exists(self, index_name: str):
         return self.es.indices.exists(index=index_name)
 
-    def _create_index(cls, index_name: str, field_name: str, num_dimensions: int):
-        if _check_index_exists(index_name=index_name):
+    def _create_index(self, index_name: str, field_name: str, num_dimensions: int):
+        if self._check_index_exists(index_name=index_name):
             raise IndexAlreadyExistsError(f"Index {index_name} already exists")
 
         mapping = {
             "mappings": {
                 "dynamic": True,
                 "_source": {"enabled": True},
                 "properties": {
                     field_name: {
                         "type": "dense_vector",
                         "dims": num_dimensions,
-                        "index": True,
+                        "index": self.index,
+                        "similarity": self.similarity
                     }
                 },
             }
         }
 
-        cls.es.indices.create(index=index_name, body=mapping)
+        self.es.indices.create(index=index_name, body=mapping)
 
     def _check_and_setup_index(
-        cls, index_name: str, field_name: str, num_dimensions: int
+        self, index_name: str, field_name: str, num_dimensions: int
     ):
-        if not _check_index_exists(index_name=index_name):
-            _create_index(
+        if not self._check_index_exists(index_name=index_name):
+            self._create_index(
                 index_name=index_name,
                 field_name=field_name,
                 num_dimensions=num_dimensions,
             )
         else:
             current_mapping = self.es.indices.get_mapping(index=index_name)
             if field_name in current_mapping[index_name]["mappings"]["properties"]:
```

### Comparing `retake-0.1.4.dev0/core/transform/embedding.py` & `retake-0.1.5.dev0/core/transform/embedding.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.4.dev0/pyproject.toml` & `retake-0.1.5.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retake"
-version = "0.1.4-dev"
+version = "0.1.5-dev"
 description = "Real-time pipelines for vectors"
 authors = ["Ming Ying <ming.ying.nyc@gmail.com>"]
 readme = "README.md"
 packages = [{include = "retake"}, {include = "core"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `retake-0.1.4.dev0/retake/embedding.py` & `retake-0.1.5.dev0/retake/embedding.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.4.dev0/retake/pipeline.py` & `retake-0.1.5.dev0/retake/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from tqdm import tqdm
-from typing import Union, Tuple
+from typing import Union, Tuple, Callable, Any
 
 from retake.embedding import OpenAIEmbedding, SentenceTransformerEmbedding
 from retake.source import PostgresSource
 from retake.transform import PostgresTransform
 from retake.sink import ElasticSearchSink
 from retake.target import ElasticSearchTarget
 from core.load.elasticsearch import ElasticSearchLoader
@@ -84,22 +84,35 @@
 
         for chunk in self.extractor.extract_all(
             relation=self.transform.relation,
             columns=self.transform.columns,
             primary_key=self.transform.primary_key,
             chunk_size=chunk_size,
         ):
-            documents = [self._apply_transform(row) for row in chunk]
-            metadata_list = [self._create_metadata(row) for row in chunk]
+            rows = chunk.get("rows")
+            primary_keys = chunk.get("primary_keys")
+
+            documents = [self._apply_transform(row) for row in rows]
+            metadata_list = [self._create_metadata(row) for row in rows]
             embeddings = self.model.create_embeddings(documents)
+            self.loader.bulk_upsert_embeddings(
+                index_name=self.target.index_name,
+                embeddings=embeddings,
+                ids=primary_keys,
+                field_name=self.target.field_name,
+                metadata=metadata_list,3
+            )
 
             progress_bar.update(chunk_size)
 
         progress_bar.close()
 
     def pipe_real_time(
-        self, cdc_server_url: str, success_webhook: str, error_webhook: str
+        self,
+        cdc_server_url: str,
+        on_success: Callable[..., Any],
+        on_error: Callable[..., Any],
     ):
         raise NotImplementedError("TODO: Implement real-time sync with CDC server")
 
     def teardown(self):
         self.extractor.teardown()
```

### Comparing `retake-0.1.4.dev0/retake/sink.py` & `retake-0.1.5.dev0/retake/sink.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.4.dev0/retake/transform.py` & `retake-0.1.5.dev0/retake/transform.py`

 * *Files identical despite different names*

### Comparing `retake-0.1.4.dev0/PKG-INFO` & `retake-0.1.5.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retake
-Version: 0.1.4.dev0
+Version: 0.1.5.dev0
 Summary: Real-time pipelines for vectors
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

