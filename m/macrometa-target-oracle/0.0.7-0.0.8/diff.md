# Comparing `tmp/macrometa-target-oracle-0.0.7.tar.gz` & `tmp/macrometa-target-oracle-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.7.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.8.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.7.tar` & `macrometa-target-oracle-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 08:11:44.346066 macrometa-target-oracle-0.0.7/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 08:11:44.346066 macrometa-target-oracle-0.0.7/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35169 2023-07-06 08:11:44.346066 macrometa-target-oracle-0.0.7/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 08:11:44.590066 macrometa-target-oracle-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.7/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 09:29:04.765838 macrometa-target-oracle-0.0.8/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 09:29:04.765838 macrometa-target-oracle-0.0.8/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35198 2023-07-06 09:29:04.765838 macrometa-target-oracle-0.0.8/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 09:29:05.041839 macrometa-target-oracle-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.8/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.8/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.7/LICENSE` & `macrometa-target-oracle-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.7/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.8/macrometa_target_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.7/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.8/macrometa_target_oracle/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,15 +523,15 @@
         Writes a batch to the SQL target. Developers may override this method
         in order to provide a more efficient upload/upsert process.
         Args:
             records: List of records to load into database.
         """
 
         key_properties = self.stream_schema_message['key_properties']
-        join_keys = list(key_properties)
+        join_keys = primary_column_names(self.stream_schema_message)
         schema = self.stream_schema_message['schema']
 
         stream_schema_message = self.stream_schema_message
         full_table_name = self.table_name(stream_schema_message['stream'], is_temporary=False)
         with self.open_connection() as connection:
             with connection.cursor() as cur:
                 cur.execute("ALTER SESSION SET TIME_ZONE = '00:00'")
@@ -595,14 +595,15 @@
             schema: Singer Schema message.
         Return:
             The number of records copied, if detectable, or `None` if the API does not
             report number of records affected/inserted.
         """
 
         columns = self.column_names()
+
         join_condition = " and ".join(
             [f"temp.{key} = target.{key}" for key in join_keys]
         )
 
         update_stmt = ", ".join(
             [
                 f"target.{key} = temp.{key}"
```

### Comparing `macrometa-target-oracle-0.0.7/pyproject.toml` & `macrometa-target-oracle-0.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.7'
+version='0.0.8'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.7/setup.py` & `macrometa-target-oracle-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.7/PKG-INFO` & `macrometa-target-oracle-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.7
+Version: 0.0.8
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

