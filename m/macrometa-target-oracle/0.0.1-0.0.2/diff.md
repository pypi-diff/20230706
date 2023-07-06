# Comparing `tmp/macrometa-target-oracle-0.0.1.tar.gz` & `tmp/macrometa-target-oracle-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.1.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.2.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.1.tar` & `macrometa-target-oracle-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 03:02:39.462988 macrometa-target-oracle-0.0.1/LICENSE
--rw-r--r--   0        0        0    23884 2023-07-06 03:02:39.466988 macrometa-target-oracle-0.0.1/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    35116 2023-07-06 03:02:39.466988 macrometa-target-oracle-0.0.1/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 03:02:39.798984 macrometa-target-oracle-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.1/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 03:38:04.490618 macrometa-target-oracle-0.0.2/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 03:38:04.490618 macrometa-target-oracle-0.0.2/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    34947 2023-07-06 03:38:04.494618 macrometa-target-oracle-0.0.2/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 03:38:04.726621 macrometa-target-oracle-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.2/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.2/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.1/LICENSE` & `macrometa-target-oracle-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.1/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.2/macrometa_target_oracle/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pkg_resources
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
 from c8connector import ConfigProperty
 from joblib import Parallel, delayed, parallel_backend
 from jsonschema import Draft7Validator, FormatChecker
 from singer import get_logger
 
-from macrometa_target_oracle.db_sync import DbSync
+from macrometa_target_oracle.db_sync import DbSync, create_wallet_file, delete_wallet_file
 
 LOGGER = get_logger('macrometa_target_oracle')
 
 DEFAULT_BATCH_SIZE_ROWS = 10000
 DEFAULT_PARALLELISM = 0  # 0 The number of threads used to flush tables
 DEFAULT_MAX_PARALLELISM = 16  # Don't use more than this number of threads by default when flushing streams in parallel
 DEFAULT_BATCH_FLUSH_INTERVAL = 60
@@ -526,22 +526,22 @@
     if args.config:
         with open(args.config) as config_input:
             config = json.load(config_input)
     else:
         config = {}
 
     try:
-        config = DbSync.create_wallet_file(config)
+        config = create_wallet_file(config)
         await setup_flush_task(config)
 
         LOGGER.debug("Exiting normally")
     except Exception as e:
-        DbSync.delete_wallet_file(config)
+        delete_wallet_file(config)
         raise e
-    DbSync.delete_wallet_file(config)
+    delete_wallet_file(config)
     return
 
 
 def main():
     """Main entry point"""
     try:
         asyncio.run(main_impl())
```

### Comparing `macrometa-target-oracle-0.0.1/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.2/macrometa_target_oracle/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 import sqlalchemy
 import time
 import uuid
 
 from collections.abc import MutableMapping
 from pathlib import Path
 from singer import get_logger
-from textwrap import dedent
 from typing import cast, Dict, List, Optional
 
 
+logger = get_logger('macrometa_target_oracle')
+
 # pylint: disable=missing-function-docstring,missing-class-docstring
 def validate_config(config):
     errors = []
     required_config_keys = [
         'host',
         'port',
         'user',
@@ -142,14 +143,57 @@
     return {
         'catalog_name': catalog_name,
         'schema_name': schema_name,
         'table_name': table_name
     }
 
 
+def create_ssl_string(ssl_string: str) -> str:
+    tls_certificate_key_list = []
+    split_string = ssl_string.split("-----")
+    if len(split_string) < 4:
+        raise Exception("Invalid PEM format for certificate.")
+    for i in range(len(split_string)):
+        if ((i % 2) == 1):
+            tls_certificate_key_list.extend(("-----", split_string[i], "-----"))
+        else:
+            tls_certificate_key_list.append(split_string[i].replace(' ', '\n'))
+    return ''.join(tls_certificate_key_list)
+
+
+def create_wallet_file(config: Dict) -> Dict:
+    path_uuid = uuid.uuid4().hex
+    path = None
+    try:
+        if config.get('ewallet_pem'):
+            path = f"/opt/oracle/config/{path_uuid}/ewallet.pem"
+            cwallet = Path(path)
+            cwallet.parent.mkdir(exist_ok=True, parents=True)
+            cwallet.write_text(create_ssl_string(config['ewallet_pem']))
+            config['ewallet_pem'] = f"/opt/oracle/config/{path_uuid}"
+            logger.info(f"ewallet.pem file created at: {path}")
+    except Exception as e:
+        logger.warn(f"Failed to create ewallet.pem file at: {path}. {e}")
+    return config
+
+
+def delete_wallet_file(config: Dict) -> None:
+    path = None
+    try:
+        if config.get('ewallet_pem'):
+            path = config['ewallet_pem'] + "/ewallet.pem"
+            cwallet = Path(path)
+            config['ewallet_pem'] = cwallet.read_text()
+            cwallet.unlink()
+            logger.info(f"ewallet.pem file deleted from: {path}")
+            cwallet.parent.rmdir()
+    except Exception as e:
+        logger.warn(f"Failed to delete ewallet.pem at: {path}. {e}")
+
+
 # pylint: disable=too-many-public-methods,too-many-instance-attributes
 class DbSync:
     def __init__(self, connection_config, stream_schema_message=None):
         """
             connection_config:      OracleDb connection details
 
             stream_schema_message:  An instance of the DbSync class is typically used to load
@@ -260,55 +304,14 @@
         dsn = "tcp://" + config["host"] + ":" + str(config["port"]) + "/" + config["service_name"]
         if config.get('ewallet_pem'):
             dsn = dsn.replace("tcp", "tcps", 1)
             dsn = f"{dsn}?wallet_location=" + config.get('ewallet_pem')
 
         return dsn
 
-    def create_ssl_string(self, ssl_string: str) -> str:
-        tls_certificate_key_list = []
-        split_string = ssl_string.split("-----")
-        if len(split_string) < 4:
-            raise Exception("Invalid PEM format for certificate.")
-        for i in range(len(split_string)):
-            if ((i % 2) == 1):
-                tls_certificate_key_list.extend(("-----", split_string[i], "-----"))
-            else:
-                tls_certificate_key_list.append(split_string[i].replace(' ', '\n'))
-
-        return ''.join(tls_certificate_key_list)
-
-    def create_wallet_file(self, config: Dict) -> Dict:
-        path_uuid = uuid.uuid4().hex
-        path = None
-        try:
-            if config.get('ewallet_pem'):
-                path = f"/opt/oracle/config/{path_uuid}/ewallet.pem"
-                cwallet = Path(path)
-                cwallet.parent.mkdir(exist_ok=True, parents=True)
-                cwallet.write_text(self.create_ssl_string(config['ewallet_pem']))
-                config['ewallet_pem'] = f"/opt/oracle/config/{path_uuid}"
-                self.logger.info(f"ewallet.pem file created at: {path}")
-        except Exception as e:
-            self.logger.warn(f"Failed to create ewallet.pem file at: {path}. {e}")
-        return config
-
-    def delete_wallet_file(self, config: Dict) -> None:
-        path = None
-        try:
-            if config.get('ewallet_pem'):
-                path = config['ewallet_pem'] + "/ewallet.pem"
-                cwallet = Path(path)
-                config['ewallet_pem'] = cwallet.read_text()
-                cwallet.unlink()
-                self.logger.info(f"ewallet.pem file deleted from: {path}")
-                cwallet.parent.rmdir()
-        except Exception as e:
-            self.logger.warn(f"Failed to delete ewallet.pem at: {path}. {e}")
-
     def open_connection(self, config):
         dsn = self.make_dsn(config)
         self.logger.info("dsn: %s", dsn)
         wallet_password = None
         wallet_location = None
         if config.get('ewallet_pem'):
             wallet_location = config["ewallet_pem"]
```

### Comparing `macrometa-target-oracle-0.0.1/pyproject.toml` & `macrometa-target-oracle-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.1'
+version='0.0.2'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.1/setup.py` & `macrometa-target-oracle-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.1/PKG-INFO` & `macrometa-target-oracle-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.1
+Version: 0.0.2
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

