# Comparing `tmp/sh-dynamodb-1.0.1.tar.gz` & `tmp/sh-dynamodb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.0.1.tar", last modified: Thu Jul  6 10:50:43 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.0.2.tar", last modified: Thu Jul  6 10:52:05 2023, max compression
```

## Comparing `sh-dynamodb-1.0.1.tar` & `sh-dynamodb-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:50:43.439247 sh-dynamodb-1.0.1/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.1/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 10:50:43.438770 sh-dynamodb-1.0.1/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.0.1/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 10:50:43.439453 sh-dynamodb-1.0.1/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 10:50:34.000000 sh-dynamodb-1.0.1/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:50:43.431770 sh-dynamodb-1.0.1/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5696 2023-07-06 10:48:33.000000 sh-dynamodb-1.0.1/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:50:43.437725 sh-dynamodb-1.0.1/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.1/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:50:43.435519 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 10:50:43.000000 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 10:50:43.000000 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 10:50:43.000000 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 10:50:43.000000 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 10:50:43.000000 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 10:50:43.000000 sh-dynamodb-1.0.1/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:52:05.868654 sh-dynamodb-1.0.2/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.2/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 10:52:05.868132 sh-dynamodb-1.0.2/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.0.2/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 10:52:05.868883 sh-dynamodb-1.0.2/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 10:52:00.000000 sh-dynamodb-1.0.2/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:52:05.862851 sh-dynamodb-1.0.2/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5696 2023-07-06 10:51:40.000000 sh-dynamodb-1.0.2/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:52:05.867270 sh-dynamodb-1.0.2/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.0.2/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:52:05.865645 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 10:52:05.000000 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 10:52:05.000000 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 10:52:05.000000 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 10:52:05.000000 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 10:52:05.000000 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 10:52:05.000000 sh-dynamodb-1.0.2/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.0.1/LICENSE` & `sh-dynamodb-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/README.md` & `sh-dynamodb-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/setup.py` & `sh-dynamodb-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.0.1",
+    version="1.0.2",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/__init__.py` & `sh-dynamodb-1.0.2/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.0.2/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/discover.py` & `sh-dynamodb-1.0.2/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.0.2/sh_dynamodb/dynamodb.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,19 @@
     """
     Setup the aws session for making the API calls
     """
 
     aws_access_key = config['access_key']
     aws_secret_access_key = config['access_secret_key']
     aws_region_name = config['region_name']
-    
+
     session = Session(
         aws_access_key=aws_access_key,
         aws_secret_access_key=aws_secret_access_key
-        region_name=aws_region_name
+        aws_region_name=aws_region_name
     )
 
     LOGGER.info("Attempting to access AWS Account")
     boto3.setup_default_session(botocore_session=refreshable_session)
 
     # if 'role_name' in config:
     #     role_arn = "arn:aws:iam::{}:role/{}".format(config['account_id'].replace('-', ''),
```

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/sync.py` & `sh-dynamodb-1.0.2/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.0.2/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.0.1/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.0.2/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*

