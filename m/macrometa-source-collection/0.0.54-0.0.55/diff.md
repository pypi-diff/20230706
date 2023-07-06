# Comparing `tmp/macrometa-source-collection-0.0.54.tar.gz` & `tmp/macrometa-source-collection-0.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.54.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.55.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.54.tar` & `macrometa-source-collection-0.0.55.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11137 2023-06-27 10:51:43.928963 macrometa-source-collection-0.0.54/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0    10263 2023-06-27 10:51:43.928963 macrometa-source-collection-0.0.54/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-27 10:51:44.192968 macrometa-source-collection-0.0.54/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.54/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.54/PKG-INFO
+-rw-r--r--   0        0        0    11137 2023-07-06 13:42:22.627178 macrometa-source-collection-0.0.55/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    10291 2023-07-06 13:42:22.627178 macrometa-source-collection-0.0.55/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-07-06 13:42:22.987179 macrometa-source-collection-0.0.55/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.55/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.55/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.54/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.55/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.54/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.55/macrometa_source_collection/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,15 @@
                     time = datetime.fromtimestamp(msg.publish_timestamp()/1000)
                     time_str = time.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
                     event_time = datetime.strptime(time_str, "%Y-%m-%dT%H:%M:%S.%fZ").replace(tzinfo=timezone.utc)
                     self.export_lag.labels(region_label, tenant_label, fabric_label, workflow_label).observe((utils.now() - event_time).total_seconds())
                 except Exception as e:
                     LOGGER.warn(f"Exception received: {e}")
                     self.export_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
+                    raise e
         
         else:
             raise FileNotFoundError("Collection {} not found".format(self._collection))
 
 
     def load_existing_data(self, stream, columns, schema_properties):
         cursor = self._c8_client._fabric.c8ql.execute(f"FOR d IN @@collection RETURN d",
@@ -158,15 +159,15 @@
                     if end_time - start_time > 10:
                         LOGGER.warn(f"Took {end_time - start_time}seconds to write record:{singer_record}")
                     self.exported_bytes.labels(region_label, tenant_label, fabric_label, workflow_label).inc(len(rec))
                     self.exported_documents.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                 else:
                     LOGGER.warn("The record: %s, does not match the most common schema. Skipping it..", rec)
         except Exception as e:
-            time.sleep(600)
+            time.sleep(100)
             raise e
 
     def send_schema_message(self, stream: CatalogEntry, bookmark_properties=[]):
         schema_message = singer.SchemaMessage(stream=stream.stream,
                                               schema=stream.schema.to_dict(),
                                               key_properties=stream.key_properties,
                                               bookmark_properties=bookmark_properties)
```

### Comparing `macrometa-source-collection-0.0.54/pyproject.toml` & `macrometa-source-collection-0.0.55/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.54'
+version='0.0.55'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.54/setup.py` & `macrometa-source-collection-0.0.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.54',
+    'version': '0.0.55',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.54/PKG-INFO` & `macrometa-source-collection-0.0.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.54
+Version: 0.0.55
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

