# Comparing `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230706083726.tar.gz` & `tmp/echofish-aws-indexing-lambda-1.0.0.dev20230706084341.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230706083726.tar", last modified: Thu Jul  6 08:38:06 2023, max compression
+gzip compressed data, was "echofish-aws-indexing-lambda-1.0.0.dev20230706084341.tar", last modified: Thu Jul  6 08:44:22 2023, max compression
```

## Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726.tar` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2101 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      703 2023-07-06 08:38:03.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.616537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.616537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12161 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 08:37:21.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:38:06.620537 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 08:38:06.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:44:22.867195 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      703 2023-07-06 08:44:19.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12209 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-06 08:43:37.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:44:22.863196 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-06 08:44:22.000000 echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/LICENSE` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230706083726
+Version: 1.0.0.dev20230706084341
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/README.md` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/setup.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-indexing-lambda",
-  version="1.0.0.dev20230706083726",
+  version="1.0.0.dev20230706084341",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-indexing-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_executor.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,16 @@
                 else:
                     break
         print(f"Deleted {counter}")
 
 
     def execute(self, message):
         session = boto3.Session()
-        dynamodb = session.client(service_name='dynamodb')
+        # dynamodb = session.client(service_name='dynamodb')
+        dynamodb = boto3.resource('dynamodb')
         #
         s3 = session.client(service_name='s3', config=botocore.config.Config(max_pool_connections=self.max_pool_connections))
         #
         start = datetime.now()  # used for benchmarking
         # Get all object in public dataset bucket
         all_objects = self.__get_all_objects(s3)
         #
```

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda/lambda_handler.py` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-indexing-lambda-1.0.0.dev20230706083726/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO` & `echofish-aws-indexing-lambda-1.0.0.dev20230706084341/src/echofish_aws_indexing_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-indexing-lambda
-Version: 1.0.0.dev20230706083726
+Version: 1.0.0.dev20230706084341
 Home-page: https://github.com/ci-cmg/echofish-aws-indexing-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

