# Comparing `tmp/macrometa-target-oracle-0.0.6.tar.gz` & `tmp/macrometa-target-oracle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.6.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.7.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.6.tar` & `macrometa-target-oracle-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 07:49:07.569947 macrometa-target-oracle-0.0.6/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 07:49:07.569947 macrometa-target-oracle-0.0.6/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35173 2023-07-06 07:49:07.569947 macrometa-target-oracle-0.0.6/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 07:49:07.817954 macrometa-target-oracle-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.6/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 08:11:44.346066 macrometa-target-oracle-0.0.7/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 08:11:44.346066 macrometa-target-oracle-0.0.7/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35169 2023-07-06 08:11:44.346066 macrometa-target-oracle-0.0.7/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 08:11:44.590066 macrometa-target-oracle-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.7/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.7/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.6/LICENSE` & `macrometa-target-oracle-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.6/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.7/macrometa_target_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.6/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.7/macrometa_target_oracle/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,17 +608,17 @@
                 f"target.{key} = temp.{key}"
                 for key in columns
                 if key not in join_keys
             ]
         )  # noqa
 
         merge_sql = f"""
-            MERGE INTO {to_table_name} AS target
-            USING {from_table_name} AS temp
-            ON {join_condition}
+            MERGE INTO {to_table_name} target
+            USING {from_table_name} temp
+            ON ({join_condition})
             WHEN MATCHED THEN
                 UPDATE SET
                     { update_stmt }
             WHEN NOT MATCHED THEN
                 INSERT ({", ".join(columns)})
                 VALUES ({", ".join([f"temp.{key}" for key in columns])});
         """  # nosec
```

### Comparing `macrometa-target-oracle-0.0.6/pyproject.toml` & `macrometa-target-oracle-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.6'
+version='0.0.7'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.6/setup.py` & `macrometa-target-oracle-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.6/PKG-INFO` & `macrometa-target-oracle-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.6
+Version: 0.0.7
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

