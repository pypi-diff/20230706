# Comparing `tmp/nhs_aws_helpers-0.1.2.tar.gz` & `tmp/nhs_aws_helpers-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_aws_helpers-0.1.2.tar", max compression
+gzip compressed data, was "nhs_aws_helpers-0.1.3.tar", max compression
```

## Comparing `nhs_aws_helpers-0.1.2.tar` & `nhs_aws_helpers-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1078 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      666 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/README.md
--rw-r--r--   0        0        0    39862 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/__init__.py
--rw-r--r--   0        0        0     7980 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/async_s3_object_reader.py
--rw-r--r--   0        0        0     6673 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/async_s3_object_writer.py
--rw-r--r--   0        0        0      674 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/common.py
--rw-r--r--   0        0        0     4095 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/fixtures.py
--rw-r--r--   0        0        0        0 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/py.typed
--rw-r--r--   0        0        0     7916 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/s3_object_reader.py
--rw-r--r--   0        0        0     6681 2023-06-26 11:16:42.772317 nhs_aws_helpers-0.1.2/nhs_aws_helpers/s3_object_writer.py
--rw-r--r--   0        0        0     3059 2023-06-26 11:17:03.835595 nhs_aws_helpers-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-26 11:16:42.776312 nhs_aws_helpers-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0    10996 2023-06-26 11:16:42.776312 nhs_aws_helpers-0.1.2/tests/async_s3_object_buffer_tests.py
--rw-r--r--   0        0        0     7558 2023-06-26 11:16:42.776312 nhs_aws_helpers-0.1.2/tests/aws_tests.py
--rw-r--r--   0        0        0      280 2023-06-26 11:16:42.776312 nhs_aws_helpers-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0    10316 2023-06-26 11:16:42.776312 nhs_aws_helpers-0.1.2/tests/s3_object_buffer_tests.py
--rw-r--r--   0        0        0      518 2023-06-26 11:16:42.776312 nhs_aws_helpers-0.1.2/tests/utils.py
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      666 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/README.md
+-rw-r--r--   0        0        0    39862 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/__init__.py
+-rw-r--r--   0        0        0     7980 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_reader.py
+-rw-r--r--   0        0        0     6673 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_writer.py
+-rw-r--r--   0        0        0      674 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/common.py
+-rw-r--r--   0        0        0     4508 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/fixtures.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/py.typed
+-rw-r--r--   0        0        0     7916 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_reader.py
+-rw-r--r--   0        0        0     6681 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_writer.py
+-rw-r--r--   0        0        0     3058 2023-07-06 21:25:40.192826 nhs_aws_helpers-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0    10996 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/async_s3_object_buffer_tests.py
+-rw-r--r--   0        0        0     7558 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/aws_tests.py
+-rw-r--r--   0        0        0      280 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0     2272 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/ddb_tests.py
+-rw-r--r--   0        0        0    10316 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/s3_object_buffer_tests.py
+-rw-r--r--   0        0        0      518 2023-07-06 21:25:18.128948 nhs_aws_helpers-0.1.3/tests/utils.py
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.1.3/PKG-INFO
```

### Comparing `nhs_aws_helpers-0.1.2/LICENSE.md` & `nhs_aws_helpers-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/README.md` & `nhs_aws_helpers-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/__init__.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/async_s3_object_reader.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/async_s3_object_writer.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/async_s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/common.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/common.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/fixtures.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/fixtures.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Generator, Tuple
+from typing import Any, Dict, Generator, Tuple
 
 import petname  # type: ignore[import]
 import pytest
 from mypy_boto3_dynamodb.service_resource import Table
 from mypy_boto3_s3.service_resource import Bucket
 from mypy_boto3_s3.type_defs import CreateBucketConfigurationTypeDef
 from mypy_boto3_sqs.service_resource import Queue
@@ -95,15 +95,15 @@
     queue = sqs.create_queue(QueueName=queue_name, Attributes=dict(FifoQueue="true", VisibilityTimeout="2"))
 
     yield queue
 
     queue.delete()
 
 
-def clone_schema(table):
+def clone_schema(table, on_demand_billing_mode: bool = True, provisioned_capacity: int = 500):
     key_schema = table.key_schema
 
     attributes = table.attribute_definitions
 
     indexes = table.global_secondary_indexes
 
     if indexes:
@@ -112,38 +112,53 @@
             del index["IndexSizeBytes"]
             del index["ItemCount"]
             del index["IndexArn"]
 
     clone = {
         "KeySchema": key_schema,
         "AttributeDefinitions": attributes,
-        "ProvisionedThroughput": {"ReadCapacityUnits": 1000, "WriteCapacityUnits": 1000},
     }
 
-    if indexes:
+    billing: Dict[str, Any] = (
+        {
+            "BillingMode": "PAY_PER_REQUEST",
+        }
+        if on_demand_billing_mode
+        else {
+            "ProvisionedThroughput": {
+                "ReadCapacityUnits": provisioned_capacity,
+                "WriteCapacityUnits": provisioned_capacity,
+            }
+        }
+    )
 
-        for index in indexes:
-            index["ProvisionedThroughput"]["ReadCapacityUnits"] = 1000
-            index["ProvisionedThroughput"]["WriteCapacityUnits"] = 1000
+    clone.update(billing)
+
+    if indexes:
+        if not on_demand_billing_mode:
+            for index in indexes:
+                index.update(billing)
         clone["GlobalSecondaryIndexes"] = indexes
 
     return clone
 
 
-def temp_dynamodb_table(source_table_name: str) -> Generator[Table, None, None]:
+def temp_dynamodb_table(
+    source_table_name: str, on_demand_billing_mode: bool = True, provisioned_capacity: int = 500
+) -> Generator[Table, None, None]:
     """
     Create a table that copies the schema of <source_table> but uses a random name, can be used throughout
     a test and is deleted at the end.
     """
     ddb = dynamodb()
 
     table_name = f"pytest-{petname.Generate(words=4, separator='_')}"
 
     source_table = ddb_table(source_table_name)
 
-    cloned = clone_schema(source_table)
+    cloned = clone_schema(source_table, on_demand_billing_mode, provisioned_capacity)
 
     table = ddb.create_table(TableName=table_name, **cloned)
 
     yield table
 
     table.delete()
```

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/s3_object_reader.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/nhs_aws_helpers/s3_object_writer.py` & `nhs_aws_helpers-0.1.3/nhs_aws_helpers/s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/pyproject.toml` & `nhs_aws_helpers-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_aws_helpers"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "nhs_aws_helpers" },
     { include = "tests", format = "sdist" },
 ]
@@ -145,15 +145,15 @@
     python --version
     which python
     pytest
 """
 
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 metadata = false
 vcs = "git"
 style = "pep440"
 format-jinja = """
     {%- if distance == 0 -%}
         {{ serialize_pep440(base, stage, revision) }}
     {%- else -%}
```

### Comparing `nhs_aws_helpers-0.1.2/tests/async_s3_object_buffer_tests.py` & `nhs_aws_helpers-0.1.3/tests/async_s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/tests/aws_tests.py` & `nhs_aws_helpers-0.1.3/tests/aws_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/tests/s3_object_buffer_tests.py` & `nhs_aws_helpers-0.1.3/tests/s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/tests/utils.py` & `nhs_aws_helpers-0.1.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.1.2/PKG-INFO` & `nhs_aws_helpers-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-aws-helpers
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: spinecore
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

