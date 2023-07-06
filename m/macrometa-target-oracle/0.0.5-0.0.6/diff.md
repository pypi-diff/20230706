# Comparing `tmp/macrometa-target-oracle-0.0.5.tar.gz` & `tmp/macrometa-target-oracle-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.5.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.6.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.5.tar` & `macrometa-target-oracle-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 05:25:35.274574 macrometa-target-oracle-0.0.5/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 05:25:35.278574 macrometa-target-oracle-0.0.5/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35214 2023-07-06 05:25:35.278574 macrometa-target-oracle-0.0.5/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 05:25:35.522578 macrometa-target-oracle-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.5/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 07:49:07.569947 macrometa-target-oracle-0.0.6/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 07:49:07.569947 macrometa-target-oracle-0.0.6/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35173 2023-07-06 07:49:07.569947 macrometa-target-oracle-0.0.6/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 07:49:07.817954 macrometa-target-oracle-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.6/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.6/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.5/LICENSE` & `macrometa-target-oracle-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.5/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.6/macrometa_target_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.5/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.6/macrometa_target_oracle/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,15 @@
         records,
         is_temp_table: bool = False,
     ):
         """Bulk insert records to an existing destination table."""
         columns = list(self.flatten_schema.keys())
 
         # Define the SQL INSERT statement
-        insert_query = f"""INSERT INTO {full_table_name} ({', '.join(columns)}) VALUES ({', '.join([f":{column}" for column in columns])})"""
+        insert_query = f"""INSERT INTO {full_table_name} VALUES ({', '.join([f":{i+1}" for i in range(len(columns))])})"""
         self.logger.info("Inserting with SQL: %s", insert_query)
 
         # Create the list of tuples for bulk insert
         values = []
         for record in records.values():
             record_values = []
             for column in columns:
@@ -594,36 +594,37 @@
             join_keys: The merge upsert keys, or `None` to append.
             schema: Singer Schema message.
         Return:
             The number of records copied, if detectable, or `None` if the API does not
             report number of records affected/inserted.
         """
 
+        columns = self.column_names()
         join_condition = " and ".join(
             [f"temp.{key} = target.{key}" for key in join_keys]
         )
 
         update_stmt = ", ".join(
             [
                 f"target.{key} = temp.{key}"
-                for key in schema["properties"].keys()
+                for key in columns
                 if key not in join_keys
             ]
         )  # noqa
 
         merge_sql = f"""
             MERGE INTO {to_table_name} AS target
             USING {from_table_name} AS temp
             ON {join_condition}
             WHEN MATCHED THEN
                 UPDATE SET
                     { update_stmt }
             WHEN NOT MATCHED THEN
-                INSERT ({", ".join(schema["properties"].keys())})
-                VALUES ({", ".join([f"temp.{key}" for key in schema["properties"].keys()])});
+                INSERT ({", ".join(columns)})
+                VALUES ({", ".join([f"temp.{key}" for key in columns])});
         """  # nosec
 
         droptable = f"DROP TABLE {from_table_name}"
         return merge_sql, droptable
 
     def column_names(self):
         return [safe_column_name(name) for name in self.flatten_schema]
```

### Comparing `macrometa-target-oracle-0.0.5/pyproject.toml` & `macrometa-target-oracle-0.0.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.5'
+version='0.0.6'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.5/setup.py` & `macrometa-target-oracle-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.5/PKG-INFO` & `macrometa-target-oracle-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.5
+Version: 0.0.6
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

