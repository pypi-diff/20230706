# Comparing `tmp/sh-dynamodb-1.4.0.tar.gz` & `tmp/sh-dynamodb-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.4.0.tar", last modified: Thu Jul  6 09:26:59 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.4.1.tar", last modified: Thu Jul  6 09:42:28 2023, max compression
```

## Comparing `sh-dynamodb-1.4.0.tar` & `sh-dynamodb-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:26:59.493799 sh-dynamodb-1.4.0/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.0/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 09:26:59.493301 sh-dynamodb-1.4.0/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.0/README.md
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:26:59.486636 sh-dynamodb-1.4.0/dz_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-05 12:15:23.000000 sh-dynamodb-1.4.0/dz_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.0/dz_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-05 10:12:23.000000 sh-dynamodb-1.4.0/dz_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5210 2023-07-05 12:46:25.000000 sh-dynamodb-1.4.0/dz_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.0/dz_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:26:59.488604 sh-dynamodb-1.4.0/dz_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.0/dz_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:04:37.000000 sh-dynamodb-1.4.0/dz_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.0/dz_dynamodb/sync_strategies/log_based.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 09:26:59.494026 sh-dynamodb-1.4.0/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 09:26:22.000000 sh-dynamodb-1.4.0/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:26:59.492498 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 09:26:59.000000 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 09:26:59.000000 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 09:26:59.000000 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 09:26:59.000000 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 09:26:59.000000 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 09:26:59.000000 sh-dynamodb-1.4.0/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.885541 sh-dynamodb-1.4.1/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.1/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 09:42:28.885002 sh-dynamodb-1.4.1/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.4.1/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 09:42:28.885752 sh-dynamodb-1.4.1/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 09:32:23.000000 sh-dynamodb-1.4.1/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.877587 sh-dynamodb-1.4.1/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5210 2023-07-05 12:46:25.000000 sh-dynamodb-1.4.1/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.883875 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.881872 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.4.0/LICENSE` & `sh-dynamodb-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.0/README.md` & `sh-dynamodb-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# dz-dynamodb
+# sh-dynamodb
 
-[![CircleCI](https://circleci.com/gh/singer-io/dz-dynamodb.svg?style=svg)](https://circleci.com/gh/singer-io/dz-dynamodb)
+[![CircleCI](https://circleci.com/gh/singer-io/sh-dynamodb.svg?style=svg)](https://circleci.com/gh/singer-io/sh-dynamodb)
 
 This is a [Singer](https://singer.io) tap that produces JSON-formatted data
 following the [Singer
 spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md).
 
 ## Configuration
```

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/__init__.py` & `sh-dynamodb-1.4.1/sh_dynamodb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import sys
 import time
 
 from terminaltables import AsciiTable
 import singer
 from singer import metadata
-from dz_dynamodb.discover import discover_streams
-from dz_dynamodb.dynamodb import setup_aws_client
-from dz_dynamodb.sync import sync_stream
+from sh_dynamodb.discover import discover_streams
+from sh_dynamodb.dynamodb import setup_aws_client
+from sh_dynamodb.sync import sync_stream
 
 
 LOGGER = singer.get_logger()
 
 REQUIRED_CONFIG_KEYS = ["region_name"]
 
 def do_discover(config):
```

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/deserialize.py` & `sh-dynamodb-1.4.1/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/discover.py` & `sh-dynamodb-1.4.1/sh_dynamodb/discover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from singer import metadata
 import singer
 from datetime import datetime
 import backoff
 from botocore.exceptions import ClientError, ConnectTimeoutError, ReadTimeoutError
-from dz_dynamodb import dynamodb
+from sh_dynamodb import dynamodb
 
 LOGGER = singer.get_logger()
 
 
 def discover_table_schema(client, table_name):
     '''
     For each of the tables in the dynamodb, create the table schema for the catalog
```

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/dynamodb.py` & `sh-dynamodb-1.4.1/sh_dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/sync.py` & `sh-dynamodb-1.4.1/sh_dynamodb/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from singer import metadata
 import singer
-from dz_dynamodb.sync_strategies import log_based
-from dz_dynamodb.sync_strategies import full_table
+from sh_dynamodb.sync_strategies import log_based
+from sh_dynamodb.sync_strategies import full_table
 
 LOGGER = singer.get_logger()
 
 def clear_state_on_replication_change(stream, state):
     md_map = metadata.to_map(stream['metadata'])
     tap_stream_id = stream['tap_stream_id']
```

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/full_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 import singer
 from singer import metadata
 import backoff
 from botocore.exceptions import ConnectTimeoutError, ReadTimeoutError
-from dz_dynamodb.deserialize import Deserializer
-from dz_dynamodb import dynamodb
+from sh_dynamodb.deserialize import Deserializer
+from sh_dynamodb import dynamodb
 
 LOGGER = singer.get_logger()
 
 
 def scan_table(table_name, projection, expression, last_evaluated_key, config):
     '''
     Get all the records of the table by using `scan()` method with projection expression parameters
@@ -83,15 +83,15 @@
     md_map = metadata.to_map(stream['metadata'])
     projection = metadata.get(md_map, (), 'tap-mongodb.projection')
     print(f"printing projection : {projection}")
 
     # An expression attribute name is a placeholder that one uses in an Amazon DynamoDB expression as an alternative to an actual attribute name.
     # Sometimes it might need to write an expression containing an attribute name that conflicts with a DynamoDB reserved word.
     # For example, table `A` contains the field `Comment` but `Comment` is a reserved word. So, it fails during fetch.
-    expression = metadata.get(md_map, (), 'dz-dynamodb.expression-attributes')
+    expression = metadata.get(md_map, (), 'sh-dynamodb.expression-attributes')
     print(f"printing expression : {expression}")
 
     rows_saved = 0
 
     deserializer = Deserializer()
     for result in scan_table(table_name, projection, expression, last_evaluated_key, config):
         for item in result.get('Items', []):
```

### Comparing `sh-dynamodb-1.4.0/dz_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/log_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 from singer import metadata
 import singer
 import backoff
 from botocore.exceptions import ConnectTimeoutError, ReadTimeoutError
-from dz_dynamodb import dynamodb, deserialize
+from sh_dynamodb import dynamodb, deserialize
 
 LOGGER = singer.get_logger()
 WRITE_STATE_PERIOD = 1000
 
 SDC_DELETED_AT = "_sdc_deleted_at"
 MAX_TRIES = 5
 FACTOR = 2
@@ -147,15 +147,15 @@
     table_name = stream['tap_stream_id']
 
     client = dynamodb.get_client(config)
     streams_client = dynamodb.get_stream_client(config)
 
     md_map = metadata.to_map(stream['metadata'])
     projection = metadata.get(md_map, (), 'tap-mongodb.projection')
-    expression = metadata.get(md_map, (), 'dz-dynamodb.expression-attributes')
+    expression = metadata.get(md_map, (), 'sh-dynamodb.expression-attributes')
     if projection is not None:
         projection = [x.strip().split('.') for x in projection.split(',')]
         if expression:
             # decode the expression in jsonified object.
             expression = dynamodb.decode_expression(expression)
             # loop over the expression keys
             for expr in expression.keys():
```

### Comparing `sh-dynamodb-1.4.0/setup.py` & `sh-dynamodb-1.4.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.4.0",
+    version="1.4.1",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
-    py_modules=["dz_dynamodb"],
+    py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
         "singer-python==5.9.0",
         'terminaltables==3.1.0',
         'backoff==1.8.0',
     ],
     extras_require={
@@ -20,13 +20,13 @@
             'ipdb',
             'pylint',
             'nose'
         ]
     },
     entry_points="""
     [console_scripts]
-    dz-dynamodb=dz_dynamodb:main
+    sh-dynamodb=sh_dynamodb:main
     """,
-    packages=["dz_dynamodb", 'dz_dynamodb.sync_strategies'],
+    packages=["sh_dynamodb", 'sh_dynamodb.sync_strategies'],
     package_data = {},
     include_package_data=True,
 )
```

