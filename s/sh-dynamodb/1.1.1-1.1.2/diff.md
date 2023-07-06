# Comparing `tmp/sh-dynamodb-1.1.1.tar.gz` & `tmp/sh-dynamodb-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.1.1.tar", last modified: Thu Jul  6 12:25:13 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.1.2.tar", last modified: Thu Jul  6 12:45:26 2023, max compression
```

## Comparing `sh-dynamodb-1.1.1.tar` & `sh-dynamodb-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:25:13.565847 sh-dynamodb-1.1.1/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.1/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:25:13.565420 sh-dynamodb-1.1.1/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.1/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 12:25:13.566022 sh-dynamodb-1.1.1/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 12:25:09.000000 sh-dynamodb-1.1.1/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:25:13.558787 sh-dynamodb-1.1.1/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5708 2023-07-06 11:45:29.000000 sh-dynamodb-1.1.1/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:25:13.564191 sh-dynamodb-1.1.1/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.1/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:25:13.562098 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:25:13.000000 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 12:25:13.000000 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 12:25:13.000000 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 12:25:13.000000 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 12:25:13.000000 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 12:25:13.000000 sh-dynamodb-1.1.1/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:45:26.574442 sh-dynamodb-1.1.2/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.2/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:45:26.574075 sh-dynamodb-1.1.2/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.2/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 12:45:26.574586 sh-dynamodb-1.1.2/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 12:43:51.000000 sh-dynamodb-1.1.2/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:45:26.569163 sh-dynamodb-1.1.2/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3315 2023-07-06 12:36:07.000000 sh-dynamodb-1.1.2/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.2/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.2/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5425 2023-07-06 12:43:14.000000 sh-dynamodb-1.1.2/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.2/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:45:26.573236 sh-dynamodb-1.1.2/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.2/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.2/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.2/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:45:26.571909 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:45:26.000000 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 12:45:26.000000 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 12:45:26.000000 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 12:45:26.000000 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 12:45:26.000000 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 12:45:26.000000 sh-dynamodb-1.1.2/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.1.1/LICENSE` & `sh-dynamodb-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.1/README.md` & `sh-dynamodb-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.1/setup.py` & `sh-dynamodb-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.1.1",
+    version="1.1.2",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/__init__.py` & `sh-dynamodb-1.1.2/sh_dynamodb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 
 
 @singer.utils.handle_top_exception(LOGGER)
 def main():
     args = singer.utils.parse_args(REQUIRED_CONFIG_KEYS)
     config = args.config
 
+    print("The config used for authenticating to AWS is : ", config)
+
     # TODO Is this the right way to do this? It seems bad
     if not config.get('use_local_dynamo'):
         setup_aws_client(config)
 
     if args.discover:
         do_discover(args.config)
     elif args.catalog:
```

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.1.2/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/discover.py` & `sh-dynamodb-1.1.2/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.1.2/sh_dynamodb/dynamodb.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,30 +43,14 @@
     def load(self):
         return DeferredRefreshableCredentials(
             self._fetcher.fetch_credentials,
             self.METHOD
         )
 
 
-# def setup_aws_client_with_access_secret_key(config):
-#     """
-#     Args : Takes config as argument 
-#     """
-
-#     aws_access_key = config['access_key']
-#     aws_secret_access_key = config['access_secret_key']
-#     aws_region_name = config['region_name']
-
-#     session = Session(
-#         aws_access_key=aws_access_key,
-#         aws_secret_access_key=aws_secret_access_key
-#         region_name=aws_region_name
-#     )
-
-
 @retry_pattern()
 def setup_aws_client(config):
     """
     Setup the aws session for making the API calls
     """
 
     # aws_access_key = config['access_key']
@@ -84,14 +68,17 @@
     # boto3.setup_default_session(botocore_session=session)
 
     if 'role_name' in config:
         role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
                                                     config['role_name'])
 
         session = Session()
+
+        print("The session credentials are : " , session.get_credentials())
+        
         fetcher = AssumeRoleCredentialFetcher(
             session.create_client,
             session.get_credentials(),
             role_arn,
             extra_args={
                 'DurationSeconds': 3600,
                 'RoleSessionName': 'TapDynamodDB',
@@ -102,14 +89,15 @@
 
         refreshable_session = Session()
         refreshable_session.register_component(
             'credential_provider',
             CredentialResolver([AssumeRoleProvider(fetcher)])
         )
 
+        print("Credentials are : ", session.get_credentials())
         LOGGER.info("Attempting to assume_role on RoleArn: %s", role_arn)
         boto3.setup_default_session(botocore_session=refreshable_session)
 
 def get_request_timeout(config):
     # if request_timeout is other than 0,"0" or "" then use request_timeout
     request_timeout = config.get('request_timeout')
     if request_timeout and float(request_timeout):
```

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/sync.py` & `sh-dynamodb-1.1.2/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.1.2/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.1.1/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.1.2/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*

