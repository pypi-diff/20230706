# Comparing `tmp/shipyard_snowflake-0.1.1a2.tar.gz` & `tmp/shipyard_snowflake-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_snowflake-0.1.1a2.tar", max compression
+gzip compressed data, was "shipyard_snowflake-0.1.1a3.tar", max compression
```

## Comparing `shipyard_snowflake-0.1.1a2.tar` & `shipyard_snowflake-0.1.1a3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349436 shipyard_snowflake-0.1.1a2/README.md
--rw-r--r--   0        0        0      684 2023-07-06 00:37:53.850026 shipyard_snowflake-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-07-05 22:46:06.931185 shipyard_snowflake-0.1.1a2/shipyard_snowflake/__init__.py
--rw-r--r--   0        0        0      606 2023-05-10 22:55:38.756415 shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/authtest.py
--rw-r--r--   0        0        0     1653 2023-07-05 22:46:06.931452 shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/execute_sql.py
--rw-r--r--   0        0        0     3159 2023-07-05 22:46:06.931699 shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/fetch.py
--rw-r--r--   0        0        0     4914 2023-07-05 22:46:06.931984 shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/upload.py
--rw-r--r--   0        0        0     5662 2023-07-05 22:46:06.932427 shipyard_snowflake-0.1.1a2/shipyard_snowflake/snowflake.py
--rw-r--r--   0        0        0     1828 2023-07-05 22:46:06.932851 shipyard_snowflake-0.1.1a2/shipyard_snowflake/test/tests.py
--rw-r--r--   0        0        0     5570 2023-07-05 22:46:06.933085 shipyard_snowflake-0.1.1a2/shipyard_snowflake/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shipyard_snowflake-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-03 22:01:51.349436 shipyard_snowflake-0.1.1a3/README.md
+-rw-r--r--   0        0        0      684 2023-07-06 13:29:35.887324 shipyard_snowflake-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-07-05 22:46:06.931185 shipyard_snowflake-0.1.1a3/shipyard_snowflake/__init__.py
+-rw-r--r--   0        0        0      605 2023-07-06 03:14:48.097910 shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/authtest.py
+-rw-r--r--   0        0        0     1726 2023-07-06 03:57:44.402546 shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/execute_sql.py
+-rw-r--r--   0        0        0     3240 2023-07-06 03:58:13.370521 shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/fetch.py
+-rw-r--r--   0        0        0     5045 2023-07-06 03:13:52.554070 shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/upload.py
+-rw-r--r--   0        0        0     5744 2023-07-06 13:23:29.267906 shipyard_snowflake-0.1.1a3/shipyard_snowflake/snowflake.py
+-rw-r--r--   0        0        0     1828 2023-07-05 22:46:06.932851 shipyard_snowflake-0.1.1a3/shipyard_snowflake/test/tests.py
+-rw-r--r--   0        0        0     5570 2023-07-05 22:46:06.933085 shipyard_snowflake-0.1.1a3/shipyard_snowflake/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 shipyard_snowflake-0.1.1a3/PKG-INFO
```

### Comparing `shipyard_snowflake-0.1.1a2/pyproject.toml` & `shipyard_snowflake-0.1.1a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-snowflake"
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = "A local client for conecting and working with Snowflake"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_snowflake"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/execute_sql.py` & `shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/execute_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         "schema": args.schema,
         "database": args.database,
         "rsa_key": None if args.private_key_path == "" else args.private_key_path,
         "role": None if args.user_role == "" else args.user_role,
     }
     client = SnowflakeClient(**client_args)
     conn = client.connect()
+    if conn == 1:
+        sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
     try:
         client.execute_query(conn=conn, query=args.query)
     except ExitCodeException as e:
         client.logger.error(e)
         sys.exit(client.EXIT_CODE_INVALID_QUERY)
```

### Comparing `shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/fetch.py` & `shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     destination_full_path = shipyard.files.combine_folder_and_file_name(
         folder_name=destination_folder_name, file_name=destination_file_name
     )
     file_header = shipyard.args.convert_to_boolean(args.file_header)
     client = SnowflakeClient(**client_args)
     try:
         conn = client.connect()
+        if conn == 1:
+            sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
     except ExitCodeException as e:
         if client_args["password"] != "":
             client.logger.error(
                 f"Ensure the password is correct for user {client_args['username']}"
             )
         if client_args["rsa_key"] != "":
             client.logger.error(
```

### Comparing `shipyard_snowflake-0.1.1a2/shipyard_snowflake/cli/upload.py` & `shipyard_snowflake-0.1.1a3/shipyard_snowflake/cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,17 @@
         not client.username and not client.rsa_key
     ):
         client.logger.error(
             "Error: Either a username and password must be provided, or a username and private key file"
         )
         sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
     conn = client.connect()  # establish connection to snowflake
+    # for authtests, connection returns 1 if unsuccessful
+    if conn == 1:
+        sys.exit(client.EXIT_CODE_INVALID_CREDENTIALS)
     if args.snowflake_data_types:
         snowflake_data_types = ast.literal_eval(args.snowflake_data_types)
     else:
         snowflake_data_types = None
 
     if args.source_file_name_match_type == "regex_match":
         # match files based on pattern
```

### Comparing `shipyard_snowflake-0.1.1a2/shipyard_snowflake/snowflake.py` & `shipyard_snowflake-0.1.1a3/shipyard_snowflake/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                 )
                 self.logger.info(f"Successfully connected to Snowflake")
                 return con
             except Exception as e:
                 self.logger.error(
                     f"Could not authenticate to Snowflake for user {self.username} with credentials in {self.rsa_key}"
                 )
+                self.logger.exception(e)
                 return 1
         else:
             try:
                 con = snowflake.connector.connect(
                     user=self.username,
                     password=self.pwd,
                     account=self.account,
@@ -86,14 +87,15 @@
                 )
                 self.logger.info(f"Successfully connected to snowflake")
                 return con
             except Exception as e:
                 self.logger.error(
                     f"Could not authenticate to account {self.account} for user {self.username}"
                 )
+                self.logger.exception(e)
                 return 1  # failed connection
 
     def upload(
         self,
         conn: snowflake.connector.SnowflakeConnection,
         df: pd.DataFrame,
         table_name: str,
```

### Comparing `shipyard_snowflake-0.1.1a2/shipyard_snowflake/test/tests.py` & `shipyard_snowflake-0.1.1a3/shipyard_snowflake/test/tests.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a2/shipyard_snowflake/utils.py` & `shipyard_snowflake-0.1.1a3/shipyard_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.1.1a2/PKG-INFO` & `shipyard_snowflake-0.1.1a3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-snowflake
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A local client for conecting and working with Snowflake
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

