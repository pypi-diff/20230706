# Comparing `tmp/blackline-postgres-0.1.1a0.tar.gz` & `tmp/blackline-postgres-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackline-postgres-0.1.1a0.tar", last modified: Wed Jun  7 13:00:17 2023, max compression
+gzip compressed data, was "blackline-postgres-0.1.2.tar", last modified: Thu Jul  6 11:50:13 2023, max compression
```

## Comparing `blackline-postgres-0.1.1a0.tar` & `blackline-postgres-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.948064 blackline-postgres-0.1.1a0/blackline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.948064 blackline-postgres-0.1.1a0/blackline/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/blackline/adapters/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/adapters/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/adapters/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.948064 blackline-postgres-0.1.1a0/blackline/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/blackline/models/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/models/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/blackline/models/postgres/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:17.000000 blackline-postgres-0.1.1a0/blackline_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-07 13:00:17.960065 blackline-postgres-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.952064 blackline-postgres-0.1.1a0/tests/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/tests/adapters/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/adapters/postgres/test_postgres_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.952064 blackline-postgres-0.1.1a0/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:17.956065 blackline-postgres-0.1.1a0/tests/models/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/models/postgres/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-07 13:00:06.000000 blackline-postgres-0.1.1a0/tests/test_postgrest_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.448097 blackline-postgres-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 11:50:13.448097 blackline-postgres-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/blackline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/blackline/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/blackline/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/blackline/adapters/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/blackline/adapters/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/blackline/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/blackline/models/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/blackline/models/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/blackline/models/postgres/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.448097 blackline-postgres-0.1.2/blackline_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 11:50:13.000000 blackline-postgres-0.1.2/blackline_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 11:50:13.000000 blackline-postgres-0.1.2/blackline_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:50:13.000000 blackline-postgres-0.1.2/blackline_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-06 11:50:13.000000 blackline-postgres-0.1.2/blackline_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 11:50:13.000000 blackline-postgres-0.1.2/blackline_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-06 11:50:13.448097 blackline-postgres-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/tests/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/tests/adapters/postgres/test_postgres_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.444097 blackline-postgres-0.1.2/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:13.448097 blackline-postgres-0.1.2/tests/models/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/tests/models/postgres/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-06 11:50:03.000000 blackline-postgres-0.1.2/tests/test_postgrest_integration.py
```

### Comparing `blackline-postgres-0.1.1a0/PKG-INFO` & `blackline-postgres-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-postgres
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core/tree/main/blackline/postgres
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-postgres-0.1.1a0/blackline/adapters/postgres/postgres.py` & `blackline-postgres-0.1.2/blackline/adapters/postgres/postgres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Union
 
 from blackline.adapters.sql.sql import SQLAdapter
 from blackline.models.collection import Column
-from blackline.models.postgres.postgres import PostgresConfig
+from blackline.models.postgres.postgres import PostgresDataStore
 from psycopg import Connection
 from psycopg.sql import SQL, Identifier
 
 
 class PostgresAdapter(SQLAdapter):
-    def __init__(self, config: PostgresConfig.Config, *args, **kwargs):
+    def __init__(self, config: PostgresDataStore.Config, *args, **kwargs):
         super().__init__(config=config, *args, **kwargs)
 
     def connection(self) -> Connection:
         conn = self.config.connection.dict()
         conninfo = conn["conninfo"]
         conn[
             "conninfo"
```

### Comparing `blackline-postgres-0.1.1a0/blackline/models/postgres/postgres.py` & `blackline-postgres-0.1.2/blackline/models/postgres/postgres.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Postgres adapter configuration. This shouldn't be here but will move is
 later and have it dynamically loaded from blackline-postgres.
 """
 
 from typing import Literal
 
-from blackline.models.adapter import AdapterConfig, ConnectionConfig
+from blackline.models.datastore_base import ConnectionConfig, DataStoreBase
 from pydantic import BaseModel, SecretStr
 
 
 class PostgresConnInfo(BaseModel):
     host: str
     port: int
     dbname: str
@@ -17,13 +17,13 @@
     password: SecretStr
 
 
 class PostgresConnectionConfig(ConnectionConfig):
     conninfo: PostgresConnInfo
 
 
-class PostgresConfig(AdapterConfig):
+class PostgresDataStore(DataStoreBase):
     class Config(BaseModel):
         connection: PostgresConnectionConfig
 
     type: Literal["postgres"]
     config: Config
```

### Comparing `blackline-postgres-0.1.1a0/blackline_postgres.egg-info/PKG-INFO` & `blackline-postgres-0.1.2/blackline_postgres.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackline-postgres
-Version: 0.1.1a0
+Version: 0.1.2
 Summary: Manage personal data in your data stores.
 Home-page: https://github.com/blacklinedata/blackline-core/tree/main/blackline/postgres
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `blackline-postgres-0.1.1a0/blackline_postgres.egg-info/SOURCES.txt` & `blackline-postgres-0.1.2/blackline_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackline-postgres-0.1.1a0/setup.cfg` & `blackline-postgres-0.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = blackline-postgres
-version = 0.1.1a0
+version = 0.1.2
 url = https://github.com/blacklinedata/blackline-core/tree/main/blackline/postgres
 description = Manage personal data in your data stores.
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Developers
@@ -20,15 +20,15 @@
 [options]
 python_requires = >=3.9, <3.12
 package_dir = 
 	=.
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	blackline-core==0.1.1a0
+	blackline-core==0.1.2
 	psycopg[binary]>=3.1
 tests_require = 
 	pytest>=6.0
 
 [options.packages.find]
 where = .
```

### Comparing `blackline-postgres-0.1.1a0/tests/adapters/postgres/test_postgres_adapter.py` & `blackline-postgres-0.1.2/tests/adapters/postgres/test_postgres_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import yaml
 from blackline.adapters.postgres.postgres import PostgresAdapter
-from blackline.models.postgres.postgres import PostgresConfig
+from blackline.models.postgres.postgres import PostgresDataStore
 from psycopg import Connection, Cursor
 from pytest import MonkeyPatch
 
 
 def test_connection(
     stores_yaml: str,
     monkeypatch: MonkeyPatch,
     postgres_connection: Connection,
     github_actions_pg: bool,
 ) -> None:
     # Setup
     store_obj = yaml.safe_load(stores_yaml)
     postgres_obj = store_obj["profiles"]["dev"]
-    pg_config = PostgresConfig.parse_obj(postgres_obj)
+    pg_config = PostgresDataStore.parse_obj(postgres_obj)
 
     if github_actions_pg:
         monkeypatch.setattr(Cursor, "fetchone", lambda self: (1,))
         monkeypatch.setattr(
             Connection, "execute", lambda self, *args, **kwargs: Cursor(self)
         )
 
@@ -126,24 +126,23 @@
             ("email", "character varying", "NO", "UNIQUE", "UNIQUE (email)", None),
             ("active", "boolean", "YES", None, None, None),
             ("name", "character varying", "YES", None, None, None),
             ("ip", "character varying", "NO", None, None, None),
             ("postal_code", "character varying", "YES", None, None, None),
         ]
 
-    table = "test_table"
     if github_actions_pg:
         monkeypatch.setattr(
             PostgresAdapter,
             "_columns_from_table",
             _columns_from_table,
         )
 
     # Run
-    columns = postgres_adapter.columns(table=table)
+    columns = postgres_adapter.columns(table=test_table)
 
     # Assert
     for column in columns:
         if column.name == "created_at":
             assert not column.nullable
             assert not column.unique
             assert not column.primary_key
```

### Comparing `blackline-postgres-0.1.1a0/tests/conftest.py` & `blackline-postgres-0.1.2/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 from typing import Callable, Generator
 
 import pytest
 import yaml
 from blackline.adapters.postgres.postgres import PostgresAdapter
 from blackline.factories.query import QueryFactory
-from blackline.models.postgres.postgres import PostgresConfig
+from blackline.models.postgres.postgres import PostgresDataStore
 from blackline.utils.testing.conftest_shared import *  # noqa: F403, F401
 from psycopg import Connection, Cursor
 from psycopg.pq import PGconn
 from psycopg.sql import SQL, Identifier
 from pytest import MonkeyPatch
 
 
@@ -129,15 +129,15 @@
         monkeypatch.setattr(Cursor, "executemany", lambda self, *args, **kwargs: None)
 
     return Connection.connect(conninfo)
 
 
 @pytest.fixture
 def load_database(
-    postgres_connection: Connection, mock_data: list, test_table: str
+    postgres_connection: Connection, mock_user_data: list, test_table: str
 ) -> Generator[Connection, None, None]:
     with postgres_connection as conn:
         with conn.cursor() as cursor:
             cursor.execute(SQL("DROP TABLE IF EXISTS {table}").format(table=test_table))
             cursor.execute(
                 SQL(
                     """
@@ -161,33 +161,37 @@
                     name,
                     email,
                     postal_code,
                     active,
                     ip
                     ) VALUES (%s, %s, %s, %s, %s, %s)"""
                 ).format(table=Identifier(test_table)),
-                mock_data,
+                mock_user_data,
             )
             conn.commit()
 
             yield conn
 
             cursor.execute(SQL("DROP TABLE IF EXISTS {table}").format(table=test_table))
 
 
 @pytest.fixture
+def postgres_datastore(stores_yaml: str) -> PostgresDataStore:
+    store_obj = yaml.safe_load(stores_yaml)
+    postgres_obj = store_obj["profiles"]["dev"]
+    return PostgresDataStore.parse_obj(postgres_obj)
+
+
+@pytest.fixture
 def postgres_adapter(
-    stores_yaml: str,
+    postgres_datastore: PostgresDataStore,
     postgres_connection: Connection,
 ) -> PostgresAdapter:
-    store_obj = yaml.safe_load(stores_yaml)
-    postgres_obj = store_obj["profiles"]["dev"]
-    pg_config = PostgresConfig.parse_obj(postgres_obj)
-    return PostgresAdapter(config=pg_config.config)
+    return PostgresAdapter(config=postgres_datastore.config)
 
 
 @pytest.fixture
 def postgres_query_factory(
     query_factory_factory: Callable,
-    postgres_adapter: PostgresAdapter,
+    postgres_datastore: PostgresDataStore,
 ) -> QueryFactory:
-    return query_factory_factory(adapter=postgres_adapter)
+    return query_factory_factory(template_params=postgres_datastore.template_params)
```

### Comparing `blackline-postgres-0.1.1a0/tests/models/postgres/test_postgres.py` & `blackline-postgres-0.1.2/tests/models/postgres/test_postgres.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import yaml
-from blackline.models.postgres.postgres import PostgresConfig
+from blackline.models.postgres.postgres import PostgresDataStore
 from pydantic.types import SecretStr
 
 
 def test_PostgresConfig(stores_yaml: str) -> None:
     # Setup
     store_obj = yaml.safe_load(stores_yaml)
     postgres_obj = store_obj["profiles"]["dev"]
 
     # Run
-    pg_config = PostgresConfig.parse_obj(postgres_obj)
+    pg_config = PostgresDataStore.parse_obj(postgres_obj)
 
     # Assert
     assert pg_config.type == "postgres"
     isinstance(pg_config.config.connection.conninfo.host, str)
     isinstance(pg_config.config.connection.conninfo.port, int)
     isinstance(pg_config.config.connection.conninfo.dbname, str)
     isinstance(pg_config.config.connection.conninfo.user, str)
```

### Comparing `blackline-postgres-0.1.1a0/tests/test_postgrest_integration.py` & `blackline-postgres-0.1.2/tests/test_postgrest_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 import os
 from typing import List
 
 import pytest
 import yaml
 from blackline.factories.query import QueryFactory
 from blackline.models.datastores import DataStore
-from blackline.models.postgres.postgres import PostgresConfig
+from blackline.models.postgres.postgres import PostgresDataStore
 from psycopg import Connection
 
 
 def test_postgrest_store_config(stores_yaml: str):
     # Setup
     pg_store_info = yaml.safe_load(stores_yaml)
 
     # Run
     store_config = DataStore.parse_obj(pg_store_info)
 
     # Assert
-    isinstance(store_config.profiles["dev"], PostgresConfig)
+    isinstance(store_config.profiles["dev"], PostgresDataStore)
 
 
 def test_query_factory_postgres_queries(
-    postgres_query_factory: QueryFactory,
+    postgres_query_factory: QueryFactory, test_table: str
 ):
     # Run
-    queries = postgres_query_factory.queries()
+    queries = tuple(postgres_query_factory.queries())
 
     # Assert
     assert (
-        queries[0].sql
-        == "UPDATE test_table\nSET\n  email = %(email_value)s,\n  name = null\nWHERE created_at < %(cutoff)s"  # noqa: E501
+        queries[0][0]
+        == f"UPDATE {test_table}\nSET\n  email = %(email_value)s,\n  name = null\nWHERE created_at < %(cutoff)s OR deactivation_date IS NOT NULL"  # noqa: E501
     )
     assert (
-        queries[1].sql
-        == "UPDATE test_table\nSET\n  ip = REGEXP_REPLACE(ip,'\\w',%(ip_value)s,'g')\nWHERE created_at < %(cutoff)s"  # noqa: E501
+        queries[1][0]
+        == f"UPDATE {test_table}\nSET\n  ip = REGEXP_REPLACE(ip,'\\w',%(ip_value)s,'g')\nWHERE created_at < %(cutoff)s OR deactivation_date IS NOT NULL"  # noqa: E501
     )
 
 
 @pytest.mark.skipif(
     os.getenv("GITHUB_ACTIONS") == "true",
     reason="Github Actions does not have a local postgres",
 )
 def test_query_factory_postgres_execution(
     load_database: Connection,
     postgres_query_factory: QueryFactory,
     test_table: str,
-    deidentified_mock_data: List,
+    deidentified_mock_user_data: List,
 ):
     # Run
     queries = postgres_query_factory.queries()
     queries[0].execute()
     queries[1].execute()
 
     # Assert
     with queries[0].adapter.connection() as conn:
         cur = conn.execute(f"SELECT * FROM {test_table}")
         rows = cur.fetchall()
 
     # Remove the id UUID from the rows
     rows = [row[1:] for row in rows]
 
-    assert set(deidentified_mock_data) == set(rows)
+    assert set(deidentified_mock_user_data) == set(rows)
```

