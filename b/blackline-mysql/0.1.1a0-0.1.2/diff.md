# Comparing `tmp/blackline-mysql-0.1.1a0.tar.gz` & `tmp/blackline-mysql-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackline-mysql-0.1.1a0.tar", last modified: Wed Jun  7 13:00:12 2023, max compression
+gzip compressed data, was "blackline-mysql-0.1.2.tar", last modified: Thu Jul  6 11:50:11 2023, max compression
```

## Comparing `blackline-mysql-0.1.1a0.tar` & `blackline-mysql-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.137747 blackline-mysql-0.1.1a0/blackline/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.137747 blackline-mysql-0.1.1a0/blackline/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/blackline/adapters/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/adapters/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/adapters/mysql/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.137747 blackline-mysql-0.1.1a0/blackline/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/blackline/models/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/models/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/blackline/models/mysql/mysql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 13:00:12.000000 blackline-mysql-0.1.1a0/blackline_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/adapters/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/adapters/mysql/test_mysql_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:00:12.141747 blackline-mysql-0.1.1a0/tests/models/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/models/mysql/test_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-07 13:00:03.000000 blackline-mysql-0.1.1a0/tests/test_mysql_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/blackline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/blackline/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/blackline/adapters/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/blackline/adapters/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/blackline/adapters/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/blackline/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/blackline/models/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/blackline/models/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/blackline/models/mysql/mysql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/blackline_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 11:50:11.000000 blackline-mysql-0.1.2/blackline_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-06 11:50:11.000000 blackline-mysql-0.1.2/blackline_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:50:11.000000 blackline-mysql-0.1.2/blackline_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 11:50:11.000000 blackline-mysql-0.1.2/blackline_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 11:50:11.000000 blackline-mysql-0.1.2/blackline_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/tests/adapters/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/tests/adapters/mysql/test_mysql_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/tests/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:50:11.408920 blackline-mysql-0.1.2/tests/models/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/tests/models/mysql/test_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 11:50:02.000000 blackline-mysql-0.1.2/tests/test_mysql_integration.py
```

### Comparing `blackline-mysql-0.1.1a0/blackline/adapters/mysql/mysql.py` & `blackline-mysql-0.1.2/blackline/adapters/mysql/mysql.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from contextlib import contextmanager
 from typing import Generator, Union
 
 from blackline.adapters.sql.sql import SQLAdapter
 from blackline.models.collection import Column
-from blackline.models.mysql.mysql import MySQLConfig
+from blackline.models.mysql.mysql import MySQLDataStore
 from mysql.connector import MySQLConnection
 
 
 class MySQLAdapter(SQLAdapter):
-    def __init__(self, config: MySQLConfig.Config, *args, **kwargs):
+    def __init__(self, config: MySQLDataStore.Config, *args, **kwargs):
         super().__init__(config=config, *args, **kwargs)
         self.database = self.config.connection.database
 
     @contextmanager
     def connection(self) -> Generator[MySQLConnection, None, None]:
         conn_args = self.config.connection.dict()
         conn_args["password"] = conn_args["password"].get_secret_value()
```

### Comparing `blackline-mysql-0.1.1a0/blackline/models/mysql/mysql.py` & `blackline-mysql-0.1.2/blackline/models/mysql/mysql.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 MySQL adapter configuration. This shouldn't be here but will move is
 later and have it dynamically loaded from blackline-postgres.
 """
 
 from typing import Literal, Optional
 
-from blackline.models.adapter import AdapterConfig, ConnectionConfig
+from blackline.models.datastore_base import ConnectionConfig, DataStoreBase
 from pydantic import BaseModel, Field, SecretStr
 
 
 class MySQLConnectionConfig(ConnectionConfig):
     user: str = Field(
         ..., description="The user name used to authenticate with the MySQL server."
     )
@@ -38,13 +38,13 @@
         None, description="The path to a Unix domain socket."
     )
 
     class Config:
         extra = "allow"
 
 
-class MySQLConfig(AdapterConfig):
+class MySQLDataStore(DataStoreBase):
     class Config(BaseModel):
         connection: MySQLConnectionConfig
 
     type: Literal["mysql"]
     config: Config
```

### Comparing `blackline-mysql-0.1.1a0/blackline_mysql.egg-info/SOURCES.txt` & `blackline-mysql-0.1.2/blackline_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackline-mysql-0.1.1a0/setup.cfg` & `blackline-mysql-0.1.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = blackline-mysql
-version = 0.1.1a0
+version = 0.1.2
 url = https://github.com/blacklinedata/blackline-core/tree/main/blackline/mysql
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
 	mysql-connector-python==8.0.32
 tests_require = 
 	pytest>=6.0
 
 [options.packages.find]
 where = .
```

### Comparing `blackline-mysql-0.1.1a0/tests/adapters/mysql/test_mysql_adapter.py` & `blackline-mysql-0.1.2/tests/adapters/mysql/test_mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `blackline-mysql-0.1.1a0/tests/conftest.py` & `blackline-mysql-0.1.2/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 from typing import Callable, Generator
 
 import pytest
 import yaml
 from blackline.adapters.mysql.mysql import MySQLAdapter
 from blackline.factories.query import QueryFactory
-from blackline.models.mysql.mysql import MySQLConfig
+from blackline.models.mysql.mysql import MySQLDataStore
 from blackline.utils.testing.conftest_shared import *  # noqa: F403, F401
 from mysql.connector import MySQLConnection
 from mysql.connector.abstracts import MySQLConnectionAbstract
 from mysql.connector.cursor import MySQLCursor
 from pytest import MonkeyPatch
 
 
@@ -133,54 +133,60 @@
         port=mysql_port,
         database=mysql_db,
     )
 
 
 @pytest.fixture
 def load_database(
-    mysql_connection: MySQLConnection, mock_data: list, test_table: str
+    mysql_connection: MySQLConnection, mock_user_data: list, test_table: str
 ) -> Generator[MySQLConnectionAbstract, None, None]:
     with mysql_connection as conn:
         with conn.cursor() as cursor:
             cursor.execute(f"DROP TABLE IF EXISTS {test_table}")
             cursor.execute(
                 f"""
                 CREATE TABLE {test_table} (
                     id CHAR(36) DEFAULT (UUID()) UNIQUE,
                     created_at TIMESTAMP,
                     name VARCHAR(255),
                     email VARCHAR(255) NOT NULL,
                     postal_code VARCHAR(15) UNIQUE,
                     active BOOLEAN,
                     ip VARCHAR(15),
+                    deactivation_date TIMESTAMP,
                     CHECK (created_at > '2020-01-01 00:00:00'),
                     PRIMARY KEY (`id`)
                     )"""
             )
             cursor.executemany(
-                f"INSERT INTO {test_table} (created_at, name, email, postal_code, active, ip) VALUES (%s, %s, %s, %s, %s, %s)",  # noqa: E501
-                mock_data,
+                f"INSERT INTO {test_table} (created_at, name, email, postal_code, active, ip, deactivation_date) VALUES (%s, %s, %s, %s, %s, %s, %s)",  # noqa: E501
+                mock_user_data,
             )
             conn.commit()
 
             yield conn
 
             cursor.execute(f"DROP TABLE IF EXISTS {test_table}")
 
 
 @pytest.fixture
+def mysql_datastore(stores_yaml: str) -> MySQLDataStore:
+    store_obj = yaml.safe_load(stores_yaml)
+    mysql_obj = store_obj["profiles"]["dev"]
+    return MySQLDataStore.parse_obj(mysql_obj)
+
+
+@pytest.fixture
 def mysql_adapter(
-    stores_yaml: str,
+    mysql_datastore: MySQLDataStore,
     mysql_connection: MySQLConnection,
 ) -> MySQLAdapter:
-    store_obj = yaml.safe_load(stores_yaml)
-    mysql_obj = store_obj["profiles"]["dev"]
-    pg_config = MySQLConfig.parse_obj(mysql_obj)
-    return MySQLAdapter(config=pg_config.config)
+    return MySQLAdapter(config=mysql_datastore.config)
 
 
 @pytest.fixture
 def mysql_query_factory(
     query_factory_factory: Callable,
     mysql_adapter: MySQLAdapter,
+    mysql_datastore: MySQLDataStore,
 ) -> QueryFactory:
-    return query_factory_factory(adapter=mysql_adapter)
+    return query_factory_factory(template_params=mysql_datastore.template_params)
```

### Comparing `blackline-mysql-0.1.1a0/tests/models/mysql/test_mysql.py` & `blackline-mysql-0.1.2/tests/models/mysql/test_mysql.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import yaml
-from blackline.models.mysql.mysql import MySQLConfig
+from blackline.models.mysql.mysql import MySQLDataStore
 from pydantic.types import SecretStr
 
 
 def test_MySQLConfig(
     stores_yaml: str,
     mysql_user: str,
     mysql_password: SecretStr,
@@ -12,15 +12,15 @@
     mysql_port: int,
 ) -> None:
     # Setup
     store_obj = yaml.safe_load(stores_yaml)
     mysql_obj = store_obj["profiles"]["dev"]
 
     # Run
-    mysql_config = MySQLConfig.parse_obj(mysql_obj)
+    mysql_config = MySQLDataStore.parse_obj(mysql_obj)
 
     # Assert
     assert mysql_config.type == "mysql"
     assert mysql_config.config.connection.host == mysql_host
     assert mysql_config.config.connection.port == mysql_port
     assert mysql_config.config.connection.database == mysql_db
     assert mysql_config.config.connection.user == mysql_user
```

### Comparing `blackline-mysql-0.1.1a0/tests/test_mysql_integration.py` & `blackline-mysql-0.1.2/tests/test_mysql_integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import os
 from typing import List
 
 import pytest
 import yaml
+from blackline.adapters.mysql.mysql import MySQLAdapter
 from blackline.factories.query import QueryFactory
 from blackline.models.datastores import DataStore
-from blackline.models.mysql.mysql import MySQLConfig
+from blackline.models.mysql.mysql import MySQLDataStore
 from mysql.connector import MySQLConnection
 
 
 def test_mysql_store_config(stores_yaml: str):
     # Setup
     pg_store_info = yaml.safe_load(stores_yaml)
 
     # Run
     store_config = DataStore.parse_obj(pg_store_info)
 
     # Assert
-    isinstance(store_config.profiles["dev"], MySQLConfig)
+    isinstance(store_config.profiles["dev"], MySQLDataStore)
 
 
 def test_query_factory_mysql_queries(
-    mysql_query_factory: QueryFactory,
+    mysql_query_factory: QueryFactory, test_table: str
 ):
     # Run
-    queries = mysql_query_factory.queries()
+    queries = tuple(mysql_query_factory.queries())
 
     # Assert
     assert (
-        queries[0].sql
-        == "UPDATE test_table\nSET\n  email = %(email_value)s,\n  name = null\nWHERE created_at < %(cutoff)s"  # noqa: E501
+        queries[0][0]
+        == f"UPDATE {test_table}\nSET\n  email = %(email_value)s,\n  name = null\nWHERE created_at < %(cutoff)s OR deactivation_date IS NOT NULL"  # noqa: E501
     )
     assert (
-        queries[1].sql
-        == "UPDATE test_table\nSET\n  ip = REGEXP_REPLACE(ip,'[:alnum:]',%(ip_value)s)\nWHERE created_at < %(cutoff)s"  # noqa: E501
+        queries[1][0]
+        == f"UPDATE {test_table}\nSET\n  ip = REGEXP_REPLACE(ip,'[:alnum:]',%(ip_value)s)\nWHERE created_at < %(cutoff)s OR deactivation_date IS NOT NULL"  # noqa: E501
     )
 
 
 @pytest.mark.skipif(
     os.getenv("GITHUB_ACTIONS") == "true",
     reason="Github Actions does not have a local mysql",
 )
 def test_query_factory_mysql_execution(
     load_database: MySQLConnection,
     mysql_query_factory: QueryFactory,
     test_table: str,
-    deidentified_mock_data: List,
+    deidentified_mock_user_data: List,
+    mysql_adapter: MySQLAdapter,
 ):
     # Run
-    queries = mysql_query_factory.queries()
-    queries[0].execute()
-    queries[1].execute()
+    queries = tuple(mysql_query_factory.queries())
+    mysql_adapter.execute(sql=queries[0][0], values=queries[0][1])
+    mysql_adapter.execute(sql=queries[1][0], values=queries[1][1])
 
     # Assert
-    with queries[0].adapter.connection() as conn:
+    with mysql_adapter.connection() as conn:
         with conn.cursor() as cursor:
             cursor.execute(f"SELECT * FROM {test_table}")
             rows = cursor.fetchall()
 
     # Remove the UUIS from the rows
     rows = [row[1:] for row in rows]
 
-    # breakpoint()
-    assert set(deidentified_mock_data) == set(rows)
+    assert set(deidentified_mock_user_data) == set(rows)
```

