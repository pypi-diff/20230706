# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418.tar", last modified: Thu Jul  6 17:55:18 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606.tar", last modified: Thu Jul  6 19:17:06 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:55:18.323048 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 17:55:18.323048 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 17:55:18.323048 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 17:55:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:55:18.319048 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:55:18.323048 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15156 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3778 2023-07-06 17:54:13.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 17:55:18.323048 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 17:55:18.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 17:55:18.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 17:55:18.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 17:55:18.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 17:55:18.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:17:06.223051 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 19:17:06.223051 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 19:17:06.223051 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-06 19:17:01.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:17:06.219051 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:17:06.223051 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15156 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3812 2023-07-06 19:16:02.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:17:06.223051 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-06 19:17:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-07-06 19:17:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 19:17:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-06 19:17:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-06 19:17:06.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706175418
+Version: 1.0.0.dev20230706191606
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230706175418",
+  version="1.0.0.dev20230706191606",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,8 +126,11 @@
         self,
         file_name,
         bucket_name,
         key,
         access_key_id=None,
         secret_access_key=None
     ):
-        self.__get_client(access_key_id, secret_access_key).upload_file(file_name, bucket_name, key)
+        self.__get_client(
+            access_key_id,
+            secret_access_key
+        ).upload_file(file_name, bucket_name, key)
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230706175418
+Version: 1.0.0.dev20230706191606
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706175418/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230706191606/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

