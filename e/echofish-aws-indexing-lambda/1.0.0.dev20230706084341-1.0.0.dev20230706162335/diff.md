# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230706084341.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230706162335.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230706084341.tar", last modified: Thu Jul  6 08:44:22 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230706162335.tar", last modified: Thu Jul  6 16:24:16 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:44:22.867195 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-06 08:44:19.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12209 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:24:16.436567 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 16:23:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 16:24:16.436567 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-07-06 16:23:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 16:24:16.436567 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-06 16:24:13.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:24:16.436567 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:24:16.436567 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 16:23:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12325 2023-07-06 16:23:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 16:23:30.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 16:24:16.436567 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 16:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-06 16:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 16:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-06 16:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 16:24:16.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230706084341
+Version: 1.0.0.dev20230706162335
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230706084341",
+  version="1.0.0.dev20230706162335",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                 df.loc[df['CRUISE'] == select_cruise, ['DATAGRAM']] = subset_datagram['DATAGRAM']
         return df.loc[df['DATAGRAM'] == 'CON0']
 
 
     def __get_calibration_information(
             self, s3
     ) -> pd.DataFrame:
-        # Calibration data generated by Chuck currently located here:
+        # Calibration data generated by data manager currently located here:
         #      https://noaa-wcsd-pds-index.s3.amazonaws.com/calibrated_crusies.csv
         response = s3.get_object(Bucket=self.calibration_bucket, Key=self.calibration_key)
         status = response.get("ResponseMetadata", {}).get("HTTPStatusCode")
         calibration_status = pd.DataFrame(columns=["DATASET_NAME", "INSTRUMENT_NAME", "CAL_STATE"])
         if status == 200:
             calibration_status = pd.read_csv(response.get("Body"))
             calibration_status['DATASET_NAME'] = calibration_status['DATASET_NAME'].apply(lambda x: x.split('_EK60')[0])
@@ -168,35 +168,40 @@
         tableKeyNames = [key.get("AttributeName") for key in table.key_schema]
         #
         #Only retrieve the keys for each item in the table (minimize data transfer)
         projectionExpression = ", ".join('#' + key for key in tableKeyNames)
         expressionAttrNames = {'#'+key: key for key in tableKeyNames}
         #
         counter = 0
-        page = table.scan(ProjectionExpression=projectionExpression, ExpressionAttributeNames=expressionAttrNames)
+        page = table.scan(
+            ProjectionExpression=projectionExpression,
+            ExpressionAttributeNames=expressionAttrNames
+        )
         with table.batch_writer() as batch:
             while page["Count"] > 0:
                 counter += page["Count"]
                 # Delete items in batches
                 for itemKeys in page["Items"]:
                     batch.delete_item(Key=itemKeys)
                 # Fetch the next page
                 if 'LastEvaluatedKey' in page:
                     page = table.scan(
-                        ProjectionExpression=projectionExpression, ExpressionAttributeNames=expressionAttrNames,
-                        ExclusiveStartKey=page['LastEvaluatedKey'])
+                        ProjectionExpression=projectionExpression,
+                        ExpressionAttributeNames=expressionAttrNames,
+                        ExclusiveStartKey=page['LastEvaluatedKey']
+                    )
                 else:
                     break
         print(f"Deleted {counter}")
 
 
     def execute(self, message):
         session = boto3.Session()
-        # dynamodb = session.client(service_name='dynamodb')
-        dynamodb = boto3.resource('dynamodb')
+        dynamodb_client = session.client(service_name='dynamodb')
+        dynamodb_resource = boto3.resource('dynamodb')
         #
         s3 = session.client(service_name='s3', config=botocore.config.Config(max_pool_connections=self.max_pool_connections))
         #
         start = datetime.now()  # used for benchmarking
         # Get all object in public dataset bucket
         all_objects = self.__get_all_objects(s3)
         #
@@ -206,15 +211,15 @@
         #
         subset_datagrams = self.__get_subset_datagrams(df=subset_ek60_by_prefix)
         print("done getting subset of datagrams")
         ek60_objects = self.__get_ek60_objects(subset_ek60_by_prefix, subset_datagrams)
         print("done getting ek60_objects")
         print(start)  # 1:26:57 to 1:39:??
         #
-        self.__truncateTable(dynamo=dynamodb, tableName=self.index_ek60_table_name)
+        self.__truncateTable(dynamo=dynamodb_resource, tableName=self.index_ek60_table_name)
         #
         calibration_status = self.__get_calibration_information(s3)
         #
         # TODO: melt calibration_status with
         # ek60_objects['CALIBRATED'] = np.repeat(False, ek60_objects.shape[0])
         # cruises = list(set(ek60_objects['CRUISE']))
         # for i in cruises:
@@ -232,15 +237,15 @@
             datagram = cruise_data['DATAGRAM'].iloc[0]
             file_count = cruise_data.shape[0]
             total_size = np.sum(cruise_data['SIZE'])
             calibrated = cruise_name in calibration_status['DATASET_NAME'].unique()  # ~276 entries
             start_date = np.min(cruise_data['DATE']).isoformat(timespec="seconds") + "Z"
             end_date = np.max(cruise_data['DATE']).isoformat(timespec="seconds") + "Z"
             #
-            dynamodb.put_item(  # TODO: verify status_code['ResponseMetadata']['HTTPStatusCode'] == 200
+            dynamodb_client.put_item(  # TODO: verify status_code['ResponseMetadata']['HTTPStatusCode'] == 200
                 TableName=self.index_ek60_table_name,
                 Item={
                     'CRUISE': {'S': cruise_name},
                     'SHIP': {'S': ship},
                     'SENSOR': {'S': sensor},
                     'DATAGRAM': {'S': datagram},
                     'FILE_COUNT': {'N': str(file_count)},
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230706162335/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230706084341
+Version: 1.0.0.dev20230706162335
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

