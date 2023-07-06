# Comparing `tmp/sh-dynamodb-1.4.1.tar.gz` & `tmp/sh-dynamodb-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh-dynamodb-1.4.1.tar", last modified: Thu Jul  6 09:42:28 2023, max compression
+gzip compressed data, was "sh-dynamodb-1.4.2.tar", last modified: Thu Jul  6 10:02:01 2023, max compression
```

## Comparing `sh-dynamodb-1.4.1.tar` & `sh-dynamodb-1.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.885541 sh-dynamodb-1.4.1/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.1/LICENSE
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 09:42:28.885002 sh-dynamodb-1.4.1/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.4.1/README.md
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 09:42:28.885752 sh-dynamodb-1.4.1/setup.cfg
--rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 09:32:23.000000 sh-dynamodb-1.4.1/setup.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.877587 sh-dynamodb-1.4.1/sh_dynamodb/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/deserialize.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/discover.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5210 2023-07-05 12:46:25.000000 sh-dynamodb-1.4.1/sh_dynamodb/dynamodb.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.883875 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/__init__.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/full_table.py
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/log_based.py
-drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 09:42:28.881872 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/entry_points.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/requires.txt
--rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 09:42:28.000000 sh-dynamodb-1.4.1/sh_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:02:01.033758 sh-dynamodb-1.4.2/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    32387 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.2/LICENSE
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 10:02:01.033425 sh-dynamodb-1.4.2/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     1372 2023-07-06 09:31:12.000000 sh-dynamodb-1.4.2/README.md
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       38 2023-07-06 10:02:01.033961 sh-dynamodb-1.4.2/setup.cfg
+-rwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)      767 2023-07-06 10:01:08.000000 sh-dynamodb-1.4.2/setup.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:02:01.026614 sh-dynamodb-1.4.2/sh_dynamodb/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3245 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4336 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/deserialize.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4057 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/discover.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     5224 2023-07-06 09:49:21.000000 sh-dynamodb-1.4.2/sh_dynamodb/dynamodb.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     3620 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/sync.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:02:01.032406 sh-dynamodb-1.4.2/sh_dynamodb/sync_strategies/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-04 06:05:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/sync_strategies/__init__.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)     4935 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/sync_strategies/full_table.py
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)    11640 2023-07-06 09:31:27.000000 sh-dynamodb-1.4.2/sh_dynamodb/sync_strategies/log_based.py
+drwxr-xr-x   0 shashankvishwakarma   (502) staff       (20)        0 2023-07-06 10:02:01.030388 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      284 2023-07-06 10:02:00.000000 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)      480 2023-07-06 10:02:00.000000 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)        1 2023-07-06 10:02:00.000000 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       60 2023-07-06 10:02:00.000000 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/entry_points.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       96 2023-07-06 10:02:00.000000 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 shashankvishwakarma   (502) staff       (20)       12 2023-07-06 10:02:00.000000 sh-dynamodb-1.4.2/sh_dynamodb.egg-info/top_level.txt
```

### Comparing `sh-dynamodb-1.4.1/LICENSE` & `sh-dynamodb-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/README.md` & `sh-dynamodb-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/setup.py` & `sh-dynamodb-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="sh-dynamodb",
-    version="1.4.1",
+    version="1.4.2",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["sh_dynamodb"],
     install_requires=[
         'boto3==1.14.9',
```

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/__init__.py` & `sh-dynamodb-1.4.2/sh_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/deserialize.py` & `sh-dynamodb-1.4.2/sh_dynamodb/deserialize.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/discover.py` & `sh-dynamodb-1.4.2/sh_dynamodb/discover.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/dynamodb.py` & `sh-dynamodb-1.4.2/sh_dynamodb/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         refreshable_session = Session()
         refreshable_session.register_component(
             'credential_provider',
             CredentialResolver([AssumeRoleProvider(fetcher)])
         )
 
-        LOGGER.info("Attempting to assume_role on RoleArn: %s", role_arn)
+        LOGGER.info("Attempting to jhbscsdcbjsdc assume_role on RoleArn: %s", role_arn)
         boto3.setup_default_session(botocore_session=refreshable_session)
 
 def get_request_timeout(config):
     # if request_timeout is other than 0,"0" or "" then use request_timeout
     request_timeout = config.get('request_timeout')
     if request_timeout and float(request_timeout):
         request_timeout = float(request_timeout)
```

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/sync.py` & `sh-dynamodb-1.4.2/sh_dynamodb/sync.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/full_table.py` & `sh-dynamodb-1.4.2/sh_dynamodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `sh-dynamodb-1.4.1/sh_dynamodb/sync_strategies/log_based.py` & `sh-dynamodb-1.4.2/sh_dynamodb/sync_strategies/log_based.py`

 * *Files identical despite different names*

