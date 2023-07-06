# Comparing `tmp/sh-dynamodb-1.0.9.tar.gz` & `tmp/sh-dynamodb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.0.9.tar", last modified: Thu Jul  6 11:33:23 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.1.0.tar", last modified: Thu Jul  6 12:17:18 2023, max compression
```

## Comparing `sh-dynamodb-1.0.9.tar` & `sh-dynamodb-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 11:33:23.908824 sh-dynamodb-1.0.9/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.9/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 11:33:23.908387 sh-dynamodb-1.0.9/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.0.9/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 11:33:23.909029 sh-dynamodb-1.0.9/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 11:33:13.000000 sh-dynamodb-1.0.9/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 11:33:23.902663 sh-dynamodb-1.0.9/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5673 2023-07-06 11:30:50.000000 sh-dynamodb-1.0.9/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 11:33:23.907447 sh-dynamodb-1.0.9/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.9/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 11:33:23.905614 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 11:33:23.000000 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 11:33:23.000000 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 11:33:23.000000 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 11:33:23.000000 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 11:33:23.000000 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 11:33:23.000000 sh-dynamodb-1.0.9/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:17:18.159321 sh-dynamodb-1.1.0/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.0/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:17:18.158920 sh-dynamodb-1.1.0/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.1.0/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 12:17:18.159531 sh-dynamodb-1.1.0/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 11:46:01.000000 sh-dynamodb-1.1.0/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:17:18.150231 sh-dynamodb-1.1.0/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5708 2023-07-06 11:45:29.000000 sh-dynamodb-1.1.0/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:17:18.157427 sh-dynamodb-1.1.0/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.1.0/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 12:17:18.154791 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 12:17:18.000000 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 12:17:18.000000 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 12:17:18.000000 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 12:17:18.000000 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 12:17:18.000000 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 12:17:18.000000 sh-dynamodb-1.1.0/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.0.9/LICENSE` & `sh-dynamodb-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/README.md` & `sh-dynamodb-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/setup.py` & `sh-dynamodb-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.0.9",
+    version="1.1.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/__init__.py` & `sh-dynamodb-1.1.0/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.1.0/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/discover.py` & `sh-dynamodb-1.1.0/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.1.0/sh_dynamodb/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,52 +65,53 @@
 
 @retry_pattern()
 def setup_aws_client(config):
     """
     Setup the aws session for making the API calls
     """
 
-    aws_access_key = config['access_key']
-    aws_secret_access_key = config['access_secret_key']
-    aws_region_name = config['region_name']
-
-    session = boto3.Session(
-        aws_access_key_id=aws_access_key,
-        aws_secret_access_key=aws_secret_access_key,
-        region_name=aws_region_name
-    )
-
-    LOGGER.info("Attempting to access AWS Account")
-    boto3.setup_default_session(session)
-
-    # if 'role_name' in config:
-    #     role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
-    #                                                 config['role_name'])
-
-        # session = Session()
-        # fetcher = AssumeRoleCredentialFetcher(
-        #     session.create_client,
-        #     session.get_credentials(),
-        #     role_arn,
-        #     extra_args={
-        #         'DurationSeconds': 3600,
-        #         'RoleSessionName': 'TapDynamodDB',
-        #         'ExternalId': config['external_id']
-        #     },
-        #     cache=JSONFileCache()
-        # )
-
-    #     refreshable_session = Session()
-    #     refreshable_session.register_component(
-    #         'credential_provider',
-    #         CredentialResolver([AssumeRoleProvider(fetcher)])
-    #     )
+    # aws_access_key = config['access_key']
+    # aws_secret_access_key = config['access_secret_key']
+    # aws_region_name = config['region_name']
+
+    # session = boto3.Session(
+    #     aws_access_key_id=aws_access_key,
+    #     aws_secret_access_key=aws_secret_access_key,
+    #     region_name=aws_region_name
+    # )
+
+    # LOGGER.info("Attempting to access AWS Account")
+    # print("the session is : ", session)
+    # boto3.setup_default_session(botocore_session=session)
+
+    if 'role_name' in config:
+        role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
+                                                    config['role_name'])
+
+        session = Session()
+        fetcher = AssumeRoleCredentialFetcher(
+            session.create_client,
+            session.get_credentials(),
+            role_arn,
+            extra_args={
+                'DurationSeconds': 3600,
+                'RoleSessionName': 'TapDynamodDB',
+                'ExternalId': config['external_id']
+            },
+            cache=JSONFileCache()
+        )
+
+        refreshable_session = Session()
+        refreshable_session.register_component(
+            'credential_provider',
+            CredentialResolver([AssumeRoleProvider(fetcher)])
+        )
 
-    #     LOGGER.info("Attempting to assume_role on RoleArn: %s", role_arn)
-    #     boto3.setup_default_session(botocore_session=refreshable_session)
+        LOGGER.info("Attempting to assume_role on RoleArn: %s", role_arn)
+        boto3.setup_default_session(botocore_session=refreshable_session)
 
 def get_request_timeout(config):
     # if request_timeout is other than 0,"0" or "" then use request_timeout
     request_timeout = config.get('request_timeout')
     if request_timeout and float(request_timeout):
         request_timeout = float(request_timeout)
     else: # If value is 0,"0" or "" then set default to 300 seconds.
```

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/sync.py` & `sh-dynamodb-1.1.0/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.1.0/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.9/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.1.0/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*

