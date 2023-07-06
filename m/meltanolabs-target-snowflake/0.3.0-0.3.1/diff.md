# Comparing `tmp/meltanolabs_target_snowflake-0.3.0.tar.gz` & `tmp/meltanolabs_target_snowflake-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.3.0.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.3.1.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.3.0.tar` & `meltanolabs_target_snowflake-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3860 2023-06-20 20:10:11.284209 meltanolabs_target_snowflake-0.3.0/LICENSE
--rw-r--r--   0        0        0     3924 2023-06-20 20:10:11.284209 meltanolabs_target_snowflake-0.3.0/README.md
--rw-r--r--   0        0        0     1282 2023-06-20 20:10:32.916325 meltanolabs_target_snowflake-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       89 2023-06-20 20:10:32.920325 meltanolabs_target_snowflake-0.3.0/target_snowflake/__init__.py
--rw-r--r--   0        0        0    18228 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/connector.py
--rw-r--r--   0        0        0     7872 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/sinks.py
--rw-r--r--   0        0        0      724 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/snowflake_types.py
--rw-r--r--   0        0        0     4057 2023-06-20 20:10:11.288209 meltanolabs_target_snowflake-0.3.0/target_snowflake/target.py
--rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3924 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/README.md
+-rw-r--r--   0        0        0     1282 2023-07-06 18:26:35.312003 meltanolabs_target_snowflake-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-06 18:26:35.316004 meltanolabs_target_snowflake-0.3.1/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    18756 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/connector.py
+-rw-r--r--   0        0        0     7872 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     4057 2023-07-06 18:26:13.815616 meltanolabs_target_snowflake-0.3.1/target_snowflake/target.py
+-rw-r--r--   0        0        0     4671 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.3.1/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.3.0/LICENSE` & `meltanolabs_target_snowflake-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.0/README.md` & `meltanolabs_target_snowflake-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.0/pyproject.toml` & `meltanolabs_target_snowflake-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.3.0"
+version = "0.3.1"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
```

### Comparing `meltanolabs_target_snowflake-0.3.0/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.3.1/target_snowflake/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from snowflake.sqlalchemy.snowdialect import SnowflakeDialect
 from sqlalchemy.engine import Engine
 from sqlalchemy.sql import text
 
 from target_snowflake.snowflake_types import NUMBER, TIMESTAMP_NTZ, VARIANT
 
 
+SNOWFLAKE_MAX_STRING_LENGTH = 16777216
+
 class TypeMap:
     def __init__(self, operator, map_value, match_value=None):
         self.operator = operator
         self.map_value = map_value
         self.match_value = match_value
 
     def match(self, compare_value):
@@ -228,30 +230,39 @@
                 "table_name": table_name,
                 "column_name": formatter.format_collation(column_name),
                 "column_type": column_type,
             },
         )
 
     @staticmethod
+    def _conform_max_length(jsonschema_type):
+        """Alter jsonschema representations to limit max length to Snowflake's VARCHAR length."""
+        max_length = jsonschema_type.get("maxLength")
+        if max_length and max_length > SNOWFLAKE_MAX_STRING_LENGTH:
+            jsonschema_type["maxLength"] = SNOWFLAKE_MAX_STRING_LENGTH
+        return jsonschema_type
+
+    @staticmethod
     def to_sql_type(jsonschema_type: dict) -> sqlalchemy.types.TypeEngine:
         """Return a JSON Schema representation of the provided type.
 
         Uses custom Snowflake types from [snowflake-sqlalchemy](https://github.com/snowflakedb/snowflake-sqlalchemy/blob/main/src/snowflake/sqlalchemy/custom_types.py)
 
         Args:
             jsonschema_type: The JSON Schema representation of the source type.
 
         Returns:
             The SQLAlchemy type representation of the data type.
         """
         # start with default implementation
+        jsonschema_type = SnowflakeConnector._conform_max_length(jsonschema_type)
         target_type = SQLConnector.to_sql_type(jsonschema_type)
         # snowflake max and default varchar length
         # https://docs.snowflake.com/en/sql-reference/intro-summary-data-types.html
-        maxlength = jsonschema_type.get("maxLength", 16777216)
+        maxlength = jsonschema_type.get("maxLength", SNOWFLAKE_MAX_STRING_LENGTH)
         # define type maps
         string_submaps = [
             TypeMap(eq, TIMESTAMP_NTZ(), "date-time"),
             TypeMap(contains, sqlalchemy.types.TIME(), "time"),
             TypeMap(eq, sqlalchemy.types.DATE(), "date"),
             TypeMap(eq, sqlalchemy.types.VARCHAR(maxlength), None),
         ]
```

### Comparing `meltanolabs_target_snowflake-0.3.0/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.3.1/target_snowflake/sinks.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.0/target_snowflake/snowflake_types.py` & `meltanolabs_target_snowflake-0.3.1/target_snowflake/snowflake_types.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.0/target_snowflake/target.py` & `meltanolabs_target_snowflake-0.3.1/target_snowflake/target.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.0/PKG-INFO` & `meltanolabs_target_snowflake-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.3.0
+Version: 0.3.1
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

