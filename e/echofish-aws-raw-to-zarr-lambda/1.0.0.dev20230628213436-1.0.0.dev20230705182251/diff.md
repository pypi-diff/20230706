# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436.tar", last modified: Wed Jun 28 21:35:47 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251.tar", last modified: Wed Jul  5 18:23:51 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 21:35:47.140991 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-28 21:35:47.140991 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 21:35:47.140991 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-28 21:35:42.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 21:35:47.136991 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 21:35:47.136991 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)     9754 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-06-28 21:34:31.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 21:35:47.136991 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-28 21:35:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-06-28 21:35:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 21:35:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 21:35:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 21:35:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:23:51.692508 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-05 18:23:51.692508 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 18:23:51.692508 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-05 18:23:47.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:23:51.692508 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:23:51.692508 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    17006 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3778 2023-07-05 18:22:46.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:23:51.692508 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-05 18:23:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-05 18:23:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 18:23:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-05 18:23:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-05 18:23:51.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230628213436
+Version: 1.0.0.dev20230705182251
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230628213436",
+  version="1.0.0.dev20230705182251",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 import boto3
 
 class DynamoOperations:
 
     def get_item(self, table_name, key):
-        response = boto3.Session().client('dynamodb').get_item(TableName=table_name, Key=key)
+        response = boto3.Session().client(service_name='dynamodb').get_item(TableName=table_name, Key=key)
         item = None
         if response['ResponseMetadata']['HTTPStatusCode'] == 200:
             if 'Item' in response:
                 item = response['Item']
         return item
 
-    def put_item(self, table_name, item):
-        response = boto3.Session().client('dynamodb').put_item(TableName=table_name, Item=item)
+    def put_item(
+        self,
+        table_name,
+        item
+    ):
+        response = boto3.Session().client(service_name='dynamodb').put_item(TableName=table_name, Item=item)
         status_code = response['ResponseMetadata']['HTTPStatusCode']
-        assert(status_code == 200), "Unable to update dynamodb table"
+        assert(status_code == 200), "Problem, unable to update dynamodb table."
 
-    def update_item(self, table_name, key, attribute_names, attribute_values, expression):
+    def update_item(
+        self,
+        table_name,
+        key,
+        expression,
+        attribute_names,
+        attribute_values
+    ):
         response = boto3.Session().client('dynamodb').update_item(
-            ExpressionAttributeNames=attribute_names,
-            ExpressionAttributeValues=attribute_values,
-            Key=key,
             TableName=table_name,
-            UpdateExpression=expression
+            Key=key,
+            UpdateExpression=expression,
+            ExpressionAttributeNames=attribute_names,
+            ExpressionAttributeValues=attribute_values
         )
         status_code = response['ResponseMetadata']['HTTPStatusCode']
-        assert(status_code == 200), "Unable to update dynamodb table"
+        assert(status_code == 200), "Problem, unable to update dynamodb table."
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import os
 import json
 from .lambda_executor import LambdaExecutor
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
 
-input_bucket=os.environ['INPUT_BUCKET']
-output_bucket=os.environ['OUTPUT_BUCKET']
-table_name=os.environ['TABLE_NAME']
-output_bucket_access_key=os.environ['OUTPUT_BUCKET_ACCESS_KEY']
-output_bucket_secret_access_key=os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
+input_bucket = os.environ['INPUT_BUCKET']  # TODO: move some of these variables to be passed in from SNS
+output_bucket = os.environ['OUTPUT_BUCKET']
+table_name = os.environ['TABLE_NAME']
+#
+output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
+output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     dynamo_operations=DynamoOperations(),
-    input_bucket=input_bucket,
-    output_bucket=output_bucket,
-    table_name=table_name,
+    #
+    # input_bucket=input_bucket, # TODO: remove
+    # output_bucket=output_bucket,
+    # table_name=table_name,
+    #
     output_bucket_access_key=output_bucket_access_key,
     output_bucket_secret_access_key=output_bucket_secret_access_key
 )
 
 def handler(sns_event, context):
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
+    # This should only ever be one message at a time...
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
         print("Start Message : " + str(message))
         executor.execute(message)
         print("Done Message : " + str(message))
     print("Done Event : " + str(sns_event))
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230628213436
+Version: 1.0.0.dev20230705182251
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230628213436/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230705182251/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

