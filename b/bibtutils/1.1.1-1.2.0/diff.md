# Comparing `tmp/bibtutils-1.1.1.tar.gz` & `tmp/bibtutils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibtutils-1.1.1.tar", last modified: Tue Mar  7 18:14:47 2023, max compression
+gzip compressed data, was "bibtutils-1.2.0.tar", last modified: Thu Jul  6 18:21:08 2023, max compression
```

## Comparing `bibtutils-1.1.1.tar` & `bibtutils-1.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:47.839005 bibtutils-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-07 18:14:36.000000 bibtutils-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:36.000000 bibtutils-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-07 18:14:47.839005 bibtutils-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-07 18:14:36.000000 bibtutils-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:47.831005 bibtutils-1.1.1/bibtutils/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:47.835005 bibtutils-1.1.1/bibtutils/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/gcp/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/gcp/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/gcp/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/gcp/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:47.839005 bibtutils-1.1.1/bibtutils/slack/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/slack/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/slack/message.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-07 18:14:36.000000 bibtutils-1.1.1/bibtutils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:47.835005 bibtutils-1.1.1/bibtutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-07 18:14:47.000000 bibtutils-1.1.1/bibtutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-07 18:14:47.000000 bibtutils-1.1.1/bibtutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 18:14:47.000000 bibtutils-1.1.1/bibtutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-07 18:14:47.000000 bibtutils-1.1.1/bibtutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-07 18:14:47.000000 bibtutils-1.1.1/bibtutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 18:14:47.000000 bibtutils-1.1.1/bibtutils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-07 18:14:36.000000 bibtutils-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-07 18:14:47.839005 bibtutils-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 18:14:36.000000 bibtutils-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:47.839005 bibtutils-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 18:14:36.000000 bibtutils-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-07 18:14:36.000000 bibtutils-1.1.1/tests/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-07 18:14:36.000000 bibtutils-1.1.1/tests/test_gcp_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-07 18:14:36.000000 bibtutils-1.1.1/tests/test_gcp_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-07 18:14:36.000000 bibtutils-1.1.1/tests/test_gcp_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-07 18:14:36.000000 bibtutils-1.1.1/tests/test_gcp_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.774853 bibtutils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 18:20:59.000000 bibtutils-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:20:59.000000 bibtutils-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-06 18:21:08.774853 bibtutils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 18:20:59.000000 bibtutils-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.766852 bibtutils-1.2.0/bibtutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.770853 bibtutils-1.2.0/bibtutils/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24430 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/gcp/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.770853 bibtutils-1.2.0/bibtutils/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/slack/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/slack/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 18:20:59.000000 bibtutils-1.2.0/bibtutils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.766852 bibtutils-1.2.0/bibtutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 18:21:08.000000 bibtutils-1.2.0/bibtutils.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 18:20:59.000000 bibtutils-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-06 18:21:08.774853 bibtutils-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 18:20:59.000000 bibtutils-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 18:21:08.770853 bibtutils-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-06 18:20:59.000000 bibtutils-1.2.0/tests/test_gcp_storage.py
```

### Comparing `bibtutils-1.1.1/LICENSE` & `bibtutils-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/PKG-INFO` & `bibtutils-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: bibtutils
-Version: 1.1.1
+Version: 1.2.0
 Summary: Functionality often used by BITS Blue Team.
 Home-page: https://github.com/broadinstitute/bibtutils
 Author: Matthew OBrien
 Author-email: mobrien@broadinstitute.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bibtutils: BITS Blue Team Utilities
 
 - **Developer**: Matthew OBrien
 - **Email**: mobrien@broadinstitute.org
```

### Comparing `bibtutils-1.1.1/README.md` & `bibtutils-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/bibtutils/gcp/bigquery.py` & `bibtutils-1.2.0/bibtutils/gcp/bigquery.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,18 +7,116 @@
 See the official BigQuery Python Client documentation here: `link <https://googleapis.dev/python/bigquery/latest/index.html>`_.
 
 """
 import logging
 
 from google.api_core import exceptions as google_exceptions
 from google.cloud import bigquery
+import re
 
 _LOGGER = logging.getLogger(__name__)
 
 
+def create_dataset(bq_project, dataset_name, description=None, location="US", credentials=None, **kwargs):
+    """
+    Creates a dataset in BigQuery using the specified parameters.
+
+    Any extra args (``kwargs``) are passed to the
+        :py:func:`gcp_bigquery:google.cloud.bigquery.client.Client.create_dataset` method.
+
+    :type bq_project: :py:class:`str`
+    :param bq_project: the project in which to find the dataset.
+
+    :type dataset_name: :py:class:`str`
+    :param dataset_name: the name of the dataset to be created.
+
+    :type description: (Optional) :py:class:`str`
+    :param description: the description for the datset. if unspecified defaults to None
+
+    :type location: (Optional) :py:class:`str`
+    :param location: if specified, creates the dataset in the desired location/region.
+        The locations and regions supported are listed in
+        #locations_and_regions. if unspoecified
+        https://cloud.google.com/bigquery/docs/locations
+        defaults to US.
+
+    :type credentials: :py:class:`google_auth:google.oauth2.credentials.Credentials`
+    :param credentials: the credentials object to use when making the API call, if not to
+        use the account running the function for authentication.
+
+    """
+    dataset_id = f"{bq_project}.{dataset_name}"
+    dataset = bigquery.Dataset(dataset_id)
+    dataset.location = location
+    dataset.description = description
+
+    _LOGGER.info(f"Attempting to create dataset: {dataset_id}")
+    _LOGGER.info("Sending dataset API request...")
+    try:
+        client = bigquery.Client(
+        project=bq_project, credentials=credentials)
+        dataset = client.create_dataset(dataset, timeout=30, **kwargs)
+        _LOGGER.info(f"Dataset created: {dataset_id}")
+    except (google_exceptions.NotFound,google_exceptions.GoogleAPICallError, google_exceptions.PermissionDenied) as e:
+        if google_exceptions.PermissionDenied:
+            _LOGGER.error(
+                "Current account does not have required permissions to create "
+                f"bigquery table in GCP project: [{bq_project}]. Navigate to "
+                f"https://console.cloud.google.com/iam-admin/iam?project={bq_project} "
+                'and add the "BigQuery User" role to the appropriate account.'
+            )
+        raise e
+    return
+
+def delete_dataset(bq_project, dataset_name, delete_contents=False, not_found_ok=False, credentials=None, **kwargs):
+    """
+    Creates a dataset in BigQuery using the specified parameters.
+
+    Any extra args (``kwargs``) are passed to the
+        :py:func:`gcp_bigquery:google.cloud.bigquery.client.Client.create_dataset` method.
+
+    :type bq_project: :py:class:`str`
+    :param bq_project: the project in which to find the dataset.
+
+    :type dataset_name: :py:class:`str`
+    :param dataset_name: the name of the dataset to be created.
+
+    :type delete_contents: (Boolean) :py:class:`str`
+    :param delete_contents: The boolean that decides to delete the dataset. if unspecified defaults to False
+        where in the dataset is not deleted if it contains tables within.
+
+    :type not_found_ok: (Boolean) :py:class:`str`
+    :param not_found_ok: Boolean used to control errors if dataset is not found. if unspecified
+        defaults to False where in errors are not suppressed.
+
+    :type credentials: :py:class:`google_auth:google.oauth2.credentials.Credentials`
+    :param credentials: the credentials object to use when making the API call, if not to
+        use the account running the function for authentication.
+
+    """
+    dataset_id = f"{bq_project}.{dataset_name}"
+
+    _LOGGER.info(f"Attempting to delete dataset: {dataset_id}")
+    _LOGGER.info("Sending dataset API request...")
+    try:
+        client = bigquery.Client(
+        project=bq_project, credentials=credentials)
+        dataset = client.delete_dataset(dataset_id, delete_contents=delete_contents, not_found_ok=not_found_ok, **kwargs)
+        _LOGGER.info(f"Dataset deleted: {dataset_id}")
+    except (google_exceptions.NotFound,google_exceptions.GoogleAPICallError, google_exceptions.PermissionDenied) as e:
+        if google_exceptions.PermissionDenied:
+            _LOGGER.error(
+                "Current account does not have required permissions to create "
+                f"bigquery table in GCP project: [{bq_project}]. Navigate to "
+                f"https://console.cloud.google.com/iam-admin/iam?project={bq_project} "
+                'and add the "BigQuery User" role to the appropriate account.'
+            )
+        raise e
+    return
+
 def create_table(
     bq_project,
     dataset,
     table,
     schema_json=[],
     time_partitioning_interval=None,
     time_partitioning_field=None,
```

### Comparing `bibtutils-1.1.1/bibtutils/gcp/iam.py` & `bibtutils-1.2.0/bibtutils/gcp/iam.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/bibtutils/gcp/pubsub.py` & `bibtutils-1.2.0/bibtutils/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/bibtutils/gcp/secrets.py` & `bibtutils-1.2.0/bibtutils/gcp/secrets.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/bibtutils/gcp/storage.py` & `bibtutils-1.2.0/bibtutils/gcp/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,49 +13,57 @@
 
 from google.api_core import exceptions as google_exceptions
 from google.cloud import storage
 
 _LOGGER = logging.getLogger(__name__)
 
 
-def create_bucket(project, bucket_name, credentials=None):
+def create_bucket(project, bucket_name, location="US", credentials=None):
     """
     Creates a Google Cloud Storage bucket in the specified project.
 
     :type project: :py:class:`str`
     :param project: the project in which to create the bucket. The account
         being used **must** have "Storage Admin" rights on **the GCP project**.
 
     :type bucket_name: :py:class:`str`
     :param bucket_name: the name of the bucket to create. Note that
         bucket names must be **universally** unique in GCP, and need to
         adhere to the GCS bucket naming guidelines:
         https://cloud.google.com/storage/docs/naming-buckets
 
+    :type location: (Optional) :py:class:`str`
+    :param location: if specified, creates the dataset in the desired location/region.
+        The locations and regions supported are listed in
+        #locations_and_regions. if unspoecified
+        https://cloud.google.com/bigquery/docs/locations
+        defaults to US.
+
     :type credentials: :py:class:`google_auth:google.oauth2.credentials.Credentials`
     :param credentials: the credentials object to use when making the API call, if not to
         use the account running the function for authentication.
 
     :rtype: :py:class:`gcp_storage:google.cloud.storage.bucket.Bucket`
     :returns:  The bucket created during this function call.
     """
     _LOGGER.info(
         f"Attempting to create bucket: [{bucket_name}] in project: [{project}]"
     )
     client = storage.Client(credentials=credentials)
     bucket = client.bucket(bucket_name)
     try:
-        bucket = client.create_bucket(bucket, project=project, location="us")
-    except google_exceptions.Forbidden as e:
-        _LOGGER.error(
-            "Current account does not have required permissions to create "
-            f"buckets in GCP project: [{project}]. Navigate to "
-            f"https://console.cloud.google.com/iam-admin/iam?project={project} "
-            'and add the "Storage Admin" role to the appropriate account.'
-        )
+        bucket = client.create_bucket(bucket, project=project, location=location)
+    except (google_exceptions.Forbidden,google_exceptions.Conflict, google_exceptions.BadRequest) as e:
+        if google_exceptions.Forbidden:
+            _LOGGER.error(
+                "Current account does not have required permissions to create "
+                f"buckets in GCP project: [{project}]. Navigate to "
+                f"https://console.cloud.google.com/iam-admin/iam?project={project} "
+                'and add the "Storage Admin" role to the appropriate account.'
+            )
         raise e
     _LOGGER.info(f"Bucket: [{bucket.name}] created successfully.")
     return bucket
 
 
 def read_gcs(bucket_name, blob_name, decode=True, credentials=None):
     """
```

### Comparing `bibtutils-1.1.1/bibtutils/slack/error.py` & `bibtutils-1.2.0/bibtutils/slack/error.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/bibtutils/slack/message.py` & `bibtutils-1.2.0/bibtutils/slack/message.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/bibtutils.egg-info/PKG-INFO` & `bibtutils-1.2.0/bibtutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: bibtutils
-Version: 1.1.1
+Version: 1.2.0
 Summary: Functionality often used by BITS Blue Team.
 Home-page: https://github.com/broadinstitute/bibtutils
 Author: Matthew OBrien
 Author-email: mobrien@broadinstitute.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bibtutils: BITS Blue Team Utilities
 
 - **Developer**: Matthew OBrien
 - **Email**: mobrien@broadinstitute.org
```

### Comparing `bibtutils-1.1.1/bibtutils.egg-info/SOURCES.txt` & `bibtutils-1.2.0/bibtutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/setup.cfg` & `bibtutils-1.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,46 @@
 [metadata]
 name = bibtutils
-version = 1.1.1
+version = 1.2.0
 author = Matthew OBrien
 author_email = mobrien@broadinstitute.org
 description = Functionality often used by BITS Blue Team.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/broadinstitute/bibtutils
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Topic :: Security
 	Topic :: Software Development :: Libraries
 	Topic :: Utilities
 
 [options]
 include_package_data = True
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	requests>=2.25
-	protobuf>=3.20
-	python-dateutil>=2.8.0
-	google-api-core>=2.7
-	google-api-python-client>=2.15
-	google-auth>=1.30
-	google-cloud-iam>=2.6
-	google-cloud-core>=2.3
-	google-cloud-storage>=1.38
-	google-cloud-bigquery>=2.18
-	google-cloud-pubsub>=2.5
-	google-cloud-secret-manager>=2.4
-	google-cloud-securitycenter>=1.3
-	googleapis-common-protos>=1.53
+	requests
+	python-dateutil
+	google-api-core
+	google-api-python-client
+	google-auth
+	google-cloud-iam
+	google-cloud-core
+	google-cloud-storage
+	google-cloud-bigquery
+	google-cloud-pubsub
+	google-cloud-secret-manager
+	google-cloud-securitycenter
+	googleapis-common-protos
+	protobuf
 zip_safe = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `bibtutils-1.1.1/tests/test_gcp_bigquery.py` & `bibtutils-1.2.0/tests/test_gcp_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 from datetime import date
 
 from .config import *
 from bibtutils.gcp import bigquery
 from bibtutils.gcp import storage
 
 
+def test_bigquery_create_dataset():
+    bigquery.create_dataset(
+        TEST_PROJECT,
+        TEST_DATASET
+    )
+
+    bigquery.delete_dataset(
+        f"{TEST_PROJECT}.{TEST_DATASET}"
+    )
+
 def test_bq_delete():
     bigquery.delete_table(
         TEST_PROJECT, TEST_DATASET, "test_delete_table", not_found_ok=True
     )
     test_schema = [
         {"name": "test_name", "mode": "REQUIRED", "type": "STRING"},
         {"name": "upload_date", "mode": "NULLABLE", "type": "DATE"},
```

### Comparing `bibtutils-1.1.1/tests/test_gcp_secrets.py` & `bibtutils-1.2.0/tests/test_gcp_secrets.py`

 * *Files identical despite different names*

### Comparing `bibtutils-1.1.1/tests/test_gcp_storage.py` & `bibtutils-1.2.0/tests/test_gcp_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,24 @@
     storage.create_bucket(TEST_PROJECT, bucket_name)
 
     # cleanup
     from google.cloud import storage as gcs
 
     gcs.Client().get_bucket(bucket_name).delete()
 
+def test_storage_create_bucket_regional():
+    bucket_name = "bibtutils-test-temp-" + str(uuid4())
+    location = "us-east4"
+    storage.create_bucket(TEST_PROJECT, bucket_name, location=location)
+
+    # cleanup
+    from google.cloud import storage as gcs
+
+    gcs.Client().get_bucket(bucket_name).delete()
+
 
 def test_storage_plaintext():
     test_timestamp = int(time.time())
     test_data = "Test data for plaintext GCS interactions."
     test_blob = f"test-gcs-plaintext-{test_timestamp}"
     storage.write_gcs(
         bucket_name=TEST_BUCKET,
```

