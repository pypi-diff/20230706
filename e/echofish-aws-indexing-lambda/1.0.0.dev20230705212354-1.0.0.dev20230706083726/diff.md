# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230705212354.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230706083726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230705212354.tar", last modified: Wed Jul  5 21:24:34 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230706083726.tar", last modified: Thu Jul  6 08:38:06 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:24:34.855781 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-05 21:23:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-07-05 21:24:34.855781 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-07-05 21:23:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 21:24:34.855781 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-05 21:24:31.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:24:34.855781 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:24:34.855781 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 21:23:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11901 2023-07-05 21:23:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-05 21:23:49.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 21:24:34.855781 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-07-05 21:24:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-07-05 21:24:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 21:24:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-05 21:24:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 21:24:34.000000 echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-06 08:38:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.616537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.616537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12161 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230705212354
+Version: 1.0.0.dev20230706083726
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230705212354",
+  version="1.0.0.dev20230706083726",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import os
 import re
 import boto3
 # import logging
 import numpy as np
 import botocore
+from botocore.config import Config
 import pandas as pd
 from datetime import datetime
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 
 # https://ncei-wcsd-archive.s3.amazonaws.com/index.html
 BUCKET_NAME = 'noaa-wcsd-pds'
 
 session = boto3.Session()
 
 dynamodb = session.client(service_name='dynamodb')
 
 max_pool_connections = 64
-client_config = botocore.config.Config(max_pool_connections=max_pool_connections)
+client_config = Config(max_pool_connections=max_pool_connections)
 s3 = session.client(service_name='s3', config=client_config)
 
 # logging.basicConfig(level=logging.DEBUG)
 # logger = logging.getLogger(__name__)
 # logger.setLevel(logging.DEBUG)
 
 # Name of dynamoDB table to hold cruise level details
-INDEX_EK60_TABLE_NAME = 'noaa-wcsd-pds-index-ek60'
+# INDEX_EK60_TABLE_NAME = 'noaa-wcsd-pds-index-ek60'
 
 
 class LambdaExecutor:
 
     def __init__(self, index_ek60_table_name, bucket_name, calibration_bucket, calibration_key):
         self.index_ek60_table_name = index_ek60_table_name
         self.input_bucket_name = bucket_name
@@ -155,23 +156,25 @@
             calibration_status['CAL_STATE'] = calibration_status['CAL_STATE'].apply(lambda x: x.find('Calibrated') >= 0)
         else:
             print(f"Unsuccessful S3 get_object response. Status - {status}")
         return calibration_status
 
 
     def __truncateTable(self, dynamo, tableName):
+        print(type(dynamo))
         table = dynamo.Table(tableName)
-
+        print(type(table))
+        #
         #get the table keys
         tableKeyNames = [key.get("AttributeName") for key in table.key_schema]
-
+        #
         #Only retrieve the keys for each item in the table (minimize data transfer)
         projectionExpression = ", ".join('#' + key for key in tableKeyNames)
         expressionAttrNames = {'#'+key: key for key in tableKeyNames}
-
+        #
         counter = 0
         page = table.scan(ProjectionExpression=projectionExpression, ExpressionAttributeNames=expressionAttrNames)
         with table.batch_writer() as batch:
             while page["Count"] > 0:
                 counter += page["Count"]
                 # Delete items in batches
                 for itemKeys in page["Items"]:
@@ -185,29 +188,33 @@
                     break
         print(f"Deleted {counter}")
 
 
     def execute(self, message):
         session = boto3.Session()
         dynamodb = session.client(service_name='dynamodb')
+        #
         s3 = session.client(service_name='s3', config=botocore.config.Config(max_pool_connections=self.max_pool_connections))
-
+        #
         start = datetime.now()  # used for benchmarking
         # Get all object in public dataset bucket
         all_objects = self.__get_all_objects(s3)
         #
         subset_ek60_by_prefix = self.__get_subset_ek60_prefix(
             df=all_objects[all_objects['Key'].str.contains('EK60')][['Key', 'Size']]
         )
+        #
         subset_datagrams = self.__get_subset_datagrams(df=subset_ek60_by_prefix)
+        print("done getting subset of datagrams")
         ek60_objects = self.__get_ek60_objects(subset_ek60_by_prefix, subset_datagrams)
+        print("done getting ek60_objects")
         print(start)  # 1:26:57 to 1:39:??
-
-        self.__truncateTable(dynamodb, self.index_ek60_table_name)
-
+        #
+        self.__truncateTable(dynamo=dynamodb, tableName=self.index_ek60_table_name)
+        #
         calibration_status = self.__get_calibration_information(s3)
         #
         # TODO: melt calibration_status with
         # ek60_objects['CALIBRATED'] = np.repeat(False, ek60_objects.shape[0])
         # cruises = list(set(ek60_objects['CRUISE']))
         # for i in cruises:
         #     print(i)
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230705212354/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230705212354
+Version: 1.0.0.dev20230706083726
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

