# Comparing `tmp/macrometa-target-oracle-0.0.4.tar.gz` & `tmp/macrometa-target-oracle-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.4.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.5.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.4.tar` & `macrometa-target-oracle-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 04:15:00.763838 macrometa-target-oracle-0.0.4/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 04:15:00.763838 macrometa-target-oracle-0.0.4/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35055 2023-07-06 04:15:00.763838 macrometa-target-oracle-0.0.4/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 04:15:01.039841 macrometa-target-oracle-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.4/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 05:25:35.274574 macrometa-target-oracle-0.0.5/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 05:25:35.278574 macrometa-target-oracle-0.0.5/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35214 2023-07-06 05:25:35.278574 macrometa-target-oracle-0.0.5/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 05:25:35.522578 macrometa-target-oracle-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.5/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.5/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.4/LICENSE` & `macrometa-target-oracle-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.4/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.5/macrometa_target_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.4/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.5/macrometa_target_oracle/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,15 @@
                 cur.execute("""ALTER SESSION SET NLS_DATE_FORMAT = 'YYYY-MM-DD"T"HH24:MI:SS."00+00:00"'""")
                 cur.execute("""ALTER SESSION SET NLS_TIMESTAMP_FORMAT='YYYY-MM-DD"T"HH24:MI:SSXFF"+00:00"'""")
                 cur.execute("""ALTER SESSION SET NLS_TIMESTAMP_TZ_FORMAT  = 'YYYY-MM-DD"T"HH24:MI:SS.FFTZH:TZM'""")
                 cur.execute(
                     query,
                     params
                 )
+                connection.commit()
                 if cur.rowcount > 0 or ignore_rowcount:
                     try:
                         return cur.fetchall()
                     except Exception as e:
                         self.logger.warn(f"Exception raised while fetching from cursor. {e}")
                 return []
 
@@ -382,15 +383,15 @@
         records,
         is_temp_table: bool = False,
     ):
         """Bulk insert records to an existing destination table."""
         columns = list(self.flatten_schema.keys())
 
         # Define the SQL INSERT statement
-        insert_query = "INSERT INTO {} ({}) VALUES ({})".format(full_table_name, ', '.join(columns), ', '.join(['%s'] * len(columns)))
+        insert_query = f"""INSERT INTO {full_table_name} ({', '.join(columns)}) VALUES ({', '.join([f":{column}" for column in columns])})"""
         self.logger.info("Inserting with SQL: %s", insert_query)
 
         # Create the list of tuples for bulk insert
         values = []
         for record in records.values():
             record_values = []
             for column in columns:
@@ -564,22 +565,24 @@
                                                 from_table_name=tmp_table_name,
                                                 to_table_name=full_table_name,
                                                 schema=schema,
                                                 join_keys=join_keys,
                                             )
                     cur.execute(merge_sql)
                     cur.execute(droptable)
+                    connection.commit()
                     self.logger.info("Merge complete.")
                 else:
                     insert_query, values = self.bulk_insert_records(
                                                 full_table_name=full_table_name,
                                                 schema=schema,
                                                 records=records,
                                             )
                     cur.executemany(insert_query, values)
+                    connection.commit()
 
     def merge_upsert_from_table(
         self,
         from_table_name: str,
         to_table_name: str,
         schema: dict,
         join_keys: List[str],
@@ -702,14 +705,15 @@
         query = "DELETE FROM {} WHERE _sdc_deleted_at IS NOT NULL".format(table)
         self.logger.info("Deleting rows from '%s' table... %s", table, query)
         with self.open_connection() as connection:
             with connection.cursor() as cur:
                 if self.connection_config.get('multitenant'):
                     cur.execute(f"ALTER SESSION SET CONTAINER = {self.connection_config.get('pdb_name', 'CDB$ROOT')}") #Switch to expected PDB
                 cur.execute(query)
+                connection.commit()
         self.logger.info("Delete query completed.")
 
     def get_tables(self):
         return self.query(
             f"SELECT table_name FROM all_tables WHERE owner = '{self.schema_name}'",
             ignore_rowcount=True
         )
```

### Comparing `macrometa-target-oracle-0.0.4/pyproject.toml` & `macrometa-target-oracle-0.0.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.4'
+version='0.0.5'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.4/setup.py` & `macrometa-target-oracle-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.4/PKG-INFO` & `macrometa-target-oracle-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.4
+Version: 0.0.5
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

