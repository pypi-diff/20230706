# Comparing `tmp/macrometa-target-oracle-0.0.2.tar.gz` & `tmp/macrometa-target-oracle-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-oracle-0.0.2.tar", max compression
+gzip compressed data, was "macrometa-target-oracle-0.0.3.tar", max compression
```

## Comparing `macrometa-target-oracle-0.0.2.tar` & `macrometa-target-oracle-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-07-06 03:38:04.490618 macrometa-target-oracle-0.0.2/LICENSE
--rw-r--r--   0        0        0    23903 2023-07-06 03:38:04.490618 macrometa-target-oracle-0.0.2/macrometa_target_oracle/__init__.py
--rw-r--r--   0        0        0    34947 2023-07-06 03:38:04.494618 macrometa-target-oracle-0.0.2/macrometa_target_oracle/db_sync.py
--rw-r--r--   0        0        0     1538 2023-07-06 03:38:04.726621 macrometa-target-oracle-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.2/setup.py
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 03:50:09.635958 macrometa-target-oracle-0.0.3/LICENSE
+-rw-r--r--   0        0        0    23903 2023-07-06 03:50:09.635958 macrometa-target-oracle-0.0.3/macrometa_target_oracle/__init__.py
+-rw-r--r--   0        0        0    35051 2023-07-06 03:50:09.635958 macrometa-target-oracle-0.0.3/macrometa_target_oracle/db_sync.py
+-rw-r--r--   0        0        0     1538 2023-07-06 03:50:09.875959 macrometa-target-oracle-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      942 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.3/setup.py
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 macrometa-target-oracle-0.0.3/PKG-INFO
```

### Comparing `macrometa-target-oracle-0.0.2/LICENSE` & `macrometa-target-oracle-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.2/macrometa_target_oracle/__init__.py` & `macrometa-target-oracle-0.0.3/macrometa_target_oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-oracle-0.0.2/macrometa_target_oracle/db_sync.py` & `macrometa-target-oracle-0.0.3/macrometa_target_oracle/db_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,26 +304,26 @@
         dsn = "tcp://" + config["host"] + ":" + str(config["port"]) + "/" + config["service_name"]
         if config.get('ewallet_pem'):
             dsn = dsn.replace("tcp", "tcps", 1)
             dsn = f"{dsn}?wallet_location=" + config.get('ewallet_pem')
 
         return dsn
 
-    def open_connection(self, config):
-        dsn = self.make_dsn(config)
+    def open_connection(self):
+        dsn = self.make_dsn(self.connection_config)
         self.logger.info("dsn: %s", dsn)
         wallet_password = None
         wallet_location = None
-        if config.get('ewallet_pem'):
-            wallet_location = config["ewallet_pem"]
-            if config.get('wallet_password'):
-                wallet_password = config["wallet_password"]
+        if self.connection_config.get('ewallet_pem'):
+            wallet_location = self.connection_config["ewallet_pem"]
+            if self.connection_config.get('wallet_password'):
+                wallet_password = self.connection_config["wallet_password"]
         return oracledb.connect(
-            user=config["user"],
-            password=config["password"],
+            user=self.connection_config["user"],
+            password=self.connection_config["password"],
             dsn=dsn,
             wallet_location=wallet_location,
             wallet_password=wallet_password,
         )
 
     def query(self, query, params=None, ignore_rowcount=False):
         self.logger.debug("Running query: %s , params: %s", query, params)
```

### Comparing `macrometa-target-oracle-0.0.2/pyproject.toml` & `macrometa-target-oracle-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-oracle"
-version='0.0.2'
+version='0.0.3'
 description = "Macrometa target connector for writing data into Oracle DB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-oracle-0.0.2/setup.py` & `macrometa-target-oracle-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-oracle = macrometa_target_oracle:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-oracle',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Macrometa target connector for writing data into Oracle DB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-oracle-0.0.2/PKG-INFO` & `macrometa-target-oracle-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-oracle
-Version: 0.0.2
+Version: 0.0.3
 Summary: Macrometa target connector for writing data into Oracle DB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,OracleDB
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

