# Comparing `tmp/cumulus-message-adapter-2.0.2.tar.gz` & `tmp/cumulus-message-adapter-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cumulus-message-adapter-2.0.2.tar", last modified: Mon Jan 10 19:42:47 2022, max compression
+gzip compressed data, was "cumulus-message-adapter-2.0.3.tar", last modified: Thu Jul  6 19:42:08 2023, max compression
```

## Comparing `cumulus-message-adapter-2.0.2.tar` & `cumulus-message-adapter-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/cumulus_message_adapter.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3374 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/cumulus_message_adapter.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      486 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/cumulus_message_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/cumulus_message_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      118 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/cumulus_message_adapter.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/cumulus_message_adapter.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/message_adapter/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3254 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/aws.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9320 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/cumulus_message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      161 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/error.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7372 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/message_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1210 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/util.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       23 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/message_adapter/version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9768 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/LICENCE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2714 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      115 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2525 2022-01-10 19:42:23.000000 cumulus-message-adapter-2.0.2/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3374 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-01-10 19:42:47.000000 cumulus-message-adapter-2.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:42:08.977559 cumulus-message-adapter-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)     9768 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/LICENCE
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-06 19:42:08.977559 cumulus-message-adapter-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5182 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:42:08.977559 cumulus-message-adapter-2.0.3/cumulus_message_adapter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-07-06 19:42:08.000000 cumulus-message-adapter-2.0.3/cumulus_message_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-06 19:42:08.000000 cumulus-message-adapter-2.0.3/cumulus_message_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 19:42:08.000000 cumulus-message-adapter-2.0.3/cumulus_message_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 19:42:08.000000 cumulus-message-adapter-2.0.3/cumulus_message_adapter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 19:42:08.000000 cumulus-message-adapter-2.0.3/cumulus_message_adapter.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:42:08.977559 cumulus-message-adapter-2.0.3/message_adapter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/aws.py
+-rw-r--r--   0 root         (0) root         (0)     9322 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/cumulus_message.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/error.py
+-rw-r--r--   0 root         (0) root         (0)     7372 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/message_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/util.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/message_adapter/version.py
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 19:42:08.977559 cumulus-message-adapter-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2525 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 19:42:08.977559 cumulus-message-adapter-2.0.3/tests/
+-rw-r--r--   0 root         (0) root         (0)    28896 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/tests/test-module.py
+-rw-r--r--   0 root         (0) root         (0)    11239 2023-07-06 19:41:58.000000 cumulus-message-adapter-2.0.3/tests/test-program.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cumulus-message-adapter-2.0.2/message_adapter/aws.py` & `cumulus-message-adapter-2.0.3/message_adapter/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Determines the correct AWS endpoint for AWS services """
 import os
 from boto3 import resource
 
 def localhost_s3_url():
     """ Returns configured LOCALSTACK_HOST url or default for localstack s3 """
     if 'LOCALSTACK_HOST' in os.environ:
-        s3_url = f"http://{os.environ['LOCALSTACK_HOST']}:4572"
+        s3_url = f"http://{os.environ['LOCALSTACK_HOST']}:4566"
     else:
-        s3_url = 'http://localhost:4572'
+        s3_url = 'http://localhost:4566'
     return s3_url
 
 
 def s3():
     """ Determines the endpoint for the S3 service """
 
     if ('CUMULUS_ENV' in os.environ) and (os.environ['CUMULUS_ENV'] == 'testing'):
```

### Comparing `cumulus-message-adapter-2.0.2/message_adapter/cumulus_message.py` & `cumulus-message-adapter-2.0.3/message_adapter/cumulus_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                           event['replace']['Key']).get()
         target_json_path = event['replace']['TargetPath']
         parsed_json_path = parse(target_json_path)
         if data is not None:
             remote_event = json.loads(data['Body'].read().decode('utf-8'))
             replacement_targets = parsed_json_path.find(event)
             if not replacement_targets or len(replacement_targets) != 1:
-                raise Exception(f'Remote event configuration target {target_json_path} invalid')
+                raise ValueError(f'Remote event configuration target {target_json_path} invalid')
             try:
                 replacement_targets[0].value.update(remote_event)
             except AttributeError:
                 parsed_json_path.update(event, remote_event)
 
             event.pop('replace')
             exception_bool = (local_exception and local_exception != 'None')
@@ -157,15 +157,15 @@
     for key in config_keys:
         if event.get(key):
             del event[key]
 
     cumulus_meta = deepcopy(event['cumulus_meta'])
     replacement_data = replace_config_values['parsed_json_path'].find(event)
     if len(replacement_data) != 1:
-        raise Exception(f'JSON path invalid: {replace_config_values["parsed_json_path"]}')
+        raise ValueError(f'JSON path invalid: {replace_config_values["parsed_json_path"]}')
     replacement_data = replacement_data[0]
 
     estimated_data_size = len(json.dumps(replacement_data.value).encode(('utf-8')))
 
     if estimated_data_size < replace_config_values['max_size']:
         return event
```

### Comparing `cumulus-message-adapter-2.0.2/message_adapter/message_adapter.py` & `cumulus-message-adapter-2.0.3/message_adapter/message_adapter.py`

 * *Files identical despite different names*

### Comparing `cumulus-message-adapter-2.0.2/message_adapter/util.py` & `cumulus-message-adapter-2.0.3/message_adapter/util.py`

 * *Files identical despite different names*

### Comparing `cumulus-message-adapter-2.0.2/LICENCE` & `cumulus-message-adapter-2.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `cumulus-message-adapter-2.0.2/setup.py` & `cumulus-message-adapter-2.0.3/setup.py`

 * *Files identical despite different names*

