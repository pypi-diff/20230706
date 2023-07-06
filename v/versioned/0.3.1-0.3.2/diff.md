# Comparing `tmp/versioned-0.3.1.tar.gz` & `tmp/versioned-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.3.1.tar", last modified: Thu Jul  6 15:40:41 2023, max compression
+gzip compressed data, was "versioned-0.3.2.tar", last modified: Thu Jul  6 16:53:41 2023, max compression
```

## Comparing `versioned-0.3.1.tar` & `versioned-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.104995 versioned-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 15:40:41.104871 versioned-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.3.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     2848 2023-07-06 15:33:50.000000 versioned-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.3.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 15:40:41.105032 versioned-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.3.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.100741 versioned-0.3.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1039 2023-07-06 15:32:11.000000 versioned-0.3.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    10000 2023-07-06 15:23:09.000000 versioned-0.3.1/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.102893 versioned-0.3.1/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.3.1/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 15:35:28.000000 versioned-0.3.1/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      330 2023-07-06 15:30:51.000000 versioned-0.3.1/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1945 2023-07-06 15:24:44.000000 versioned-0.3.1/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.3.1/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    16712 2023-07-06 15:21:05.000000 versioned-0.3.1/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.103587 versioned-0.3.1/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.3.1/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.3.1/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.103978 versioned-0.3.1/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.3.1/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.104687 versioned-0.3.1/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.3.1/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.103481 versioned-0.3.1/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.151189 versioned-0.3.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.3.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.3.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.3.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 16:53:41.151031 versioned-0.3.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.3.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3152 2023-07-06 16:52:53.000000 versioned-0.3.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.3.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.3.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.3.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.3.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.3.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 16:53:41.151232 versioned-0.3.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.3.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.146201 versioned-0.3.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1058 2023-07-06 16:52:28.000000 versioned-0.3.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10092 2023-07-06 16:50:27.000000 versioned-0.3.2/tests/test_core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.148740 versioned-0.3.2/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.3.2/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 16:51:24.000000 versioned-0.3.2/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      295 2023-07-06 16:22:35.000000 versioned-0.3.2/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1864 2023-07-06 16:43:17.000000 versioned-0.3.2/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      181 2023-07-06 16:33:04.000000 versioned-0.3.2/versioned/constants.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16380 2023-07-06 16:48:54.000000 versioned-0.3.2/versioned/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.149530 versioned-0.3.2/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.3.2/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.3.2/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.149999 versioned-0.3.2/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.3.2/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.150810 versioned-0.3.2/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.3.2/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.3.2/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 16:53:41.149397 versioned-0.3.2/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 16:53:41.000000 versioned-0.3.2/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.3.1/AUTHORS.rst` & `versioned-0.3.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/LICENSE.txt` & `versioned-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/PKG-INFO` & `versioned-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.3.1
+Version: 0.3.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.3.1/README.rst` & `versioned-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/release-history.rst` & `versioned-0.3.2/release-history.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.2 (2023-07-06)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- now the ``versioned.api.Repository`` takes explicit ``aws_region``, ``s3_bucket`` arguments in constructor.
+- add ``versioned.api.Repository.get_artifact_s3path`` to public API.
+
+
 0.3.1 (2023-07-06)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - Created a new public API class ``versioned.api.Repository``, allow developer to customize the S3 bucket and DynamoDB table name backend. So old API are renamed to:
     - ``versioned.api.Repository.bootstrap``
     - ``versioned.api.Repository.put_artifact``
```

### Comparing `versioned-0.3.1/requirements-doc.txt` & `versioned-0.3.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/setup.py` & `versioned-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/tests/test_api.py` & `versioned-0.3.2/tests/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from versioned import api
 
 
 def test():
     _ = api
     _ = api.exc
     _ = api.DYNAMODB_TABLE_NAME
-    _ = api.BUCKET_NAME
     _ = api.S3_PREFIX
     _ = api.LATEST_VERSION
     _ = api.VERSION_ZFILL
     _ = api.Artifact
     _ = api.Alias
     _ = api.Repository
+    _ = api.Repository.get_artifact_s3path
     _ = api.Repository.put_artifact
     _ = api.Repository.get_artifact_version
     _ = api.Repository.list_artifact_versions
     _ = api.Repository.publish_artifact_version
     _ = api.Repository.delete_artifact_version
     _ = api.Repository.put_alias
     _ = api.Repository.get_alias
```

### Comparing `versioned-0.3.1/tests/test_core.py` & `versioned-0.3.2/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import moto
 import pytest
 
 from s3pathlib import S3Path, context
 
 from versioned import exc
 from versioned import constants
-from versioned.bootstrap import bootstrap
 from versioned.dynamodb import encode_version
 from versioned.tests.mock_aws import BaseMockTest
 from versioned.core import Repository
 
 from rich import print as rprint
 
 
@@ -25,15 +24,18 @@
     ]
 
     repo: Repository = None
 
     @classmethod
     def setup_class_post_hook(cls):
         context.attach_boto_session(cls.bsm.boto_ses)
-        cls.repo = Repository()
+        cls.repo = Repository(
+            aws_region=cls.bsm.aws_region,
+            s3_bucket=f"{cls.bsm.aws_account_id}-{cls.bsm.aws_region}-artifacts",
+        )
         cls.repo.bootstrap(cls.bsm)
 
     def _test(self):
         name = "deploy"
         alias = "LIVE"
 
         self.repo.purge_artifact(bsm=self.bsm, name=name)
```

### Comparing `versioned-0.3.1/versioned/bootstrap.py` & `versioned-0.3.2/versioned/bootstrap.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pynamodb.models import PAY_PER_REQUEST_BILLING_MODE
 from pynamodb.connection import Connection
 from . import dynamodb
 
 
 def bootstrap(
     bsm: BotoSesManager,
+    aws_region: str,
     bucket_name: str,
     dynamodb_table_name: str,
     dynamodb_write_capacity_units: T.Optional[int] = None,
     dynamodb_read_capacity_units: T.Optional[int] = None,
 ):
     """
     Bootstrap the associated AWS account and region in the boto session manager.
@@ -31,17 +32,14 @@
         ]
     ) not in [
         0,
         2,
     ]:  # pragma: no cover
         raise ValueError
 
-    aws_account_id = bsm.sts_client.get_caller_identity()["Account"]
-    aws_region = bsm.aws_region
-
     # create s3 bucket
     try:
         bsm.s3_client.head_bucket(Bucket=bucket_name)
     except Exception as e:
         if "Not Found" in str(e):
             bsm.s3_client.create_bucket(Bucket=bucket_name)
         else:
```

### Comparing `versioned-0.3.1/versioned/core.py` & `versioned-0.3.2/versioned/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import dataclasses
 from datetime import datetime
 
 from boto_session_manager import BotoSesManager
 from s3pathlib import S3Path
 from func_args import NOTHING
+from pynamodb.connection import Connection
 
 from . import constants
 from . import dynamodb
 from . import exc
 from .bootstrap import bootstrap
 from .vendor.hashes import hashes
 
@@ -103,92 +104,90 @@
         Get the content of the secondary artifact version of this alias.
         """
         return self.s3path_secondary_version.read_bytes(bsm=bsm)
 
 
 @dataclasses.dataclass
 class Repository:
-    s3_bucket: T.Optional[str] = dataclasses.field(default=None)
-    s3_prefix: T.Optional[str] = dataclasses.field(default=constants.S3_PREFIX)
-    dynamodb_table_name: T.Optional[str] = dataclasses.field(
-        default=constants.DYNAMODB_TABLE_NAME
-    )
-
-    def _get_s3_bucket(self, bsm: BotoSesManager) -> str:
-        if self.s3_bucket is None:
-            return f"{bsm.aws_account_id}-{bsm.aws_region}-{constants.BUCKET_NAME}"
-        else:
-            return self.s3_bucket
+    aws_region: str = dataclasses.field()
+    s3_bucket: str = dataclasses.field()
+    s3_prefix: str = dataclasses.field(default=constants.S3_PREFIX)
+    dynamodb_table_name: str = dataclasses.field(default=constants.DYNAMODB_TABLE_NAME)
 
-    def _get_s3path(self, bsm: BotoSesManager, name: str, version: str) -> S3Path:
-        return S3Path(self._get_s3_bucket(bsm=bsm)).joinpath(
+    @property
+    def s3dir_artifact_store(self) -> S3Path:
+        """
+        Return the s3dir of the artifact store folder.
+        """
+        return S3Path(self.s3_bucket).joinpath(self.s3_prefix).to_dir()
+
+    def get_artifact_s3path(self, name: str, version: str) -> S3Path:
+        return S3Path(self.s3_bucket).joinpath(
             self.s3_prefix,
             name,
             dynamodb.encode_version(version),
         )
 
     def bootstrap(
         self,
         bsm: BotoSesManager,
         dynamodb_write_capacity_units: T.Optional[int] = None,
         dynamodb_read_capacity_units: T.Optional[int] = None,
     ):
         bootstrap(
             bsm=bsm,
-            bucket_name=self._get_s3_bucket(bsm=bsm),
+            aws_region=self.aws_region,
+            bucket_name=self.s3_bucket,
             dynamodb_table_name=self.dynamodb_table_name,
             dynamodb_write_capacity_units=dynamodb_write_capacity_units,
             dynamodb_read_capacity_units=dynamodb_read_capacity_units,
         )
 
-    def _get_artifact_class(self, bsm: BotoSesManager) -> T.Type[dynamodb.Artifact]:
+    @property
+    def _artifact_class(self) -> T.Type[dynamodb.Artifact]:
         class Artifact(dynamodb.Artifact):
             class Meta:
                 table_name = self.dynamodb_table_name
-                region = bsm.aws_region
+                region = self.aws_region
 
         return Artifact
 
-    def _get_alias_class(self, bsm: BotoSesManager) -> T.Type[dynamodb.Alias]:
+    @property
+    def _alias_class(self) -> T.Type[dynamodb.Alias]:
         class Alias(dynamodb.Alias):
             class Meta:
                 table_name = self.dynamodb_table_name
-                region = bsm.aws_region
+                region = self.aws_region
 
         return Alias
 
     def _get_artifact_object(
         self,
-        bsm: BotoSesManager,
         artifact: dynamodb.Artifact,
     ) -> Artifact:
         dct = artifact.to_dict()
-        dct["s3uri"] = self._get_s3path(
-            bsm=bsm,
+        dct["s3uri"] = self.get_artifact_s3path(
             name=artifact.name,
             version=artifact.version,
         ).uri
         return Artifact(**dct)
 
     def _get_alias_object(
         self,
-        bsm: BotoSesManager,
         alias: dynamodb.Alias,
     ) -> Alias:
         dct = alias.to_dict()
-        dct["version_s3uri"] = self._get_s3path(
-            bsm=bsm,
+        dct["version_s3uri"] = self.get_artifact_s3path(
             name=alias.name,
             version=alias.version,
         ).uri
         if alias.secondary_version is None:
             dct["secondary_version_s3uri"] = None
         else:
-            dct["secondary_version_s3uri"] = self._get_s3path(
-                bsm=bsm,
+            dct["secondary_version_s3uri"] = self.get_artifact_s3path(
                 name=alias.name,
                 version=alias.secondary_version,
             ).uri
         return Alias(**dct)
 
     # ------------------------------------------------------------------------------
     # Artifact
@@ -207,24 +206,23 @@
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         :param content: binary artifact content.
         :param metadata: optional metadata of the s3 object.
         :param tags: optional tags of the s3 object.
         """
-        Artifact = self._get_artifact_class(bsm)
-        artifact = Artifact.new(name=name)
+        artifact = self._artifact_class.new(name=name)
         artifact_sha256 = hashes.of_bytes(content)
         artifact.sha256 = artifact_sha256
-        s3path = self._get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
+        s3path = self.get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
 
         # do nothing if the content is not changed
         if s3path.exists(bsm=bsm):
             if s3path.metadata["artifact_sha256"] == artifact_sha256:
-                return self._get_artifact_object(bsm=bsm, artifact=artifact)
+                return self._get_artifact_object(artifact=artifact)
 
         final_metadata = dict(
             artifact_name=name,
             artifact_sha256=artifact_sha256,
         )
         if metadata is not NOTHING:
             final_metadata.update(metadata)
@@ -232,15 +230,15 @@
             content,
             metadata=final_metadata,
             content_type=content_type,
             tags=tags,
             bsm=bsm,
         )
         artifact.save()
-        return self._get_artifact_object(bsm=bsm, artifact=artifact)
+        return self._get_artifact_object(artifact=artifact)
 
     def _get_artifact_dynamodb_item(
         self,
         artifact_class: T.Type[dynamodb.Artifact],
         name: str,
         version: T.Union[int, str],
     ) -> dynamodb.Artifact:
@@ -266,37 +264,38 @@
         """
         Return the information about the artifact or artifact version.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         :param version: artifact version. If ``None``, return the latest version.
         """
-        Artifact = self._get_artifact_class(bsm)
         if version is None:
             version = constants.LATEST_VERSION
         artifact = self._get_artifact_dynamodb_item(
-            Artifact, name=name, version=version
+            self._artifact_class,
+            name=name,
+            version=version,
         )
-        return self._get_artifact_object(bsm=bsm, artifact=artifact)
+        return self._get_artifact_object(artifact=artifact)
 
     def list_artifact_versions(
         self,
         bsm: BotoSesManager,
         name: str,
     ) -> T.List[Artifact]:
         """
         Return a list of artifact versions. The latest version is always the first item.
         And the newer version comes first.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        Artifact = self._get_artifact_class(bsm)
+        Artifact = self._artifact_class
         return [
-            self._get_artifact_object(bsm=bsm, artifact=artifact)
+            self._get_artifact_object(artifact=artifact)
             for artifact in Artifact.query(
                 hash_key=name,
                 scan_index_forward=False,
                 filter_condition=Artifact.is_deleted == False,
             )
         ]
 
@@ -308,33 +307,33 @@
         """
         Creates a version from the latest artifact. Use versions to create an
         immutable snapshot of your latest artifact.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        Artifact = self._get_artifact_class(bsm)
+        Artifact = self._artifact_class
         artifacts = list(
             Artifact.query(hash_key=name, scan_index_forward=False, limit=2)
         )
         if len(artifacts) == 0:
             raise exc.ArtifactNotFoundError(f"name = {name!r}")
         elif len(artifacts) == 1:
             new_version = "1"
         else:
             new_version = str(int(artifacts[1].version) + 1)
         artifact = Artifact.new(name=name, version=new_version)
         artifact.sha256 = artifacts[0].sha256
         artifact.save()
-        s3path_old = self._get_s3path(
-            bsm=bsm, name=name, version=constants.LATEST_VERSION
+        s3path_old = self.get_artifact_s3path(
+            name=name, version=constants.LATEST_VERSION,
         )
-        s3path_new = self._get_s3path(bsm=bsm, name=name, version=new_version)
+        s3path_new = self.get_artifact_s3path(name=name, version=new_version)
         s3path_old.copy_to(s3path_new, bsm=bsm)
-        return self._get_artifact_object(bsm=bsm, artifact=artifact)
+        return self._get_artifact_object(artifact=artifact)
 
     def delete_artifact_version(
         self,
         bsm: BotoSesManager,
         name: str,
         version: T.Optional[T.Union[int, str]] = None,
     ):
@@ -344,15 +343,15 @@
         neither the S3 artifact nor the DynamoDB item is deleted. It is just
         become "invisible" to the :func:`get_artifact` and :func:`list_artifacts``.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         :param version: artifact version. If ``None``, delete the latest version.
         """
-        Artifact = self._get_artifact_class(bsm)
+        Artifact = self._artifact_class
         if version is None:
             version = constants.LATEST_VERSION
         res = Artifact.new(name=name, version=version).update(
             actions=[
                 Artifact.is_deleted.set(True),
             ],
         )
@@ -392,52 +391,53 @@
         if secondary_version is not None:
             if not isinstance(secondary_version_weight, int):
                 raise TypeError("secondary_version_weight must be int")
             if not (0 <= secondary_version_weight < 100):
                 raise ValueError("secondary_version_weight must be 0 <= x < 100")
 
         # ensure the artifact exists
-        Artifact = self._get_artifact_class(bsm)
+        Artifact = self._artifact_class
         if version is None:
             version = constants.LATEST_VERSION
         self._get_artifact_dynamodb_item(Artifact, name=name, version=version)
         if secondary_version is not None:
             self._get_artifact_dynamodb_item(
-                Artifact, name=name, version=secondary_version
+                Artifact,
+                name=name,
+                version=secondary_version,
             )
 
-        Alias = self._get_alias_class(bsm)
+        Alias = self._alias_class
         alias = Alias.new(
             name=name,
             alias=alias,
             version=version,
             secondary_version=secondary_version,
             secondary_version_weight=secondary_version_weight,
         )
 
         alias.save()
-        return self._get_alias_object(bsm=bsm, alias=alias)
+        return self._get_alias_object(alias=alias)
 
     def get_alias(
         self,
         bsm: BotoSesManager,
         name: str,
         alias: str,
     ) -> Alias:
         """
         Return details about the alias.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         :param alias: alias name. alias name cannot have hyphen
         """
-        Alias = self._get_alias_class(bsm)
+        Alias = self._alias_class
         try:
             return self._get_alias_object(
-                bsm=bsm,
                 alias=Alias.get(
                     hash_key=dynamodb.encode_alias_key(name),
                     range_key=alias,
                 ),
             )
         except Alias.DoesNotExist:
             raise exc.AliasNotFoundError(f"name = {name!r}, alias = {alias!r}")
@@ -449,31 +449,30 @@
     ) -> T.List[Alias]:
         """
         Returns a list of aliases for an artifact.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        Alias = self._get_alias_class(bsm)
+        Alias = self._alias_class
         return [
-            self._get_alias_object(bsm=bsm, alias=alias)
+            self._get_alias_object(alias=alias)
             for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name))
         ]
 
     def delete_alias(
         self,
         bsm: BotoSesManager,
         name: str,
         alias: str,
     ):
         """
         Deletes an alias.
         """
-        Alias = self._get_alias_class(bsm)
-        res = Alias.new(name=name, alias=alias).delete()
+        res = self._alias_class.new(name=name, alias=alias).delete()
         # print(res)
 
     def purge_artifact(
         self,
         bsm: BotoSesManager,
         name: str,
     ):
@@ -481,19 +480,19 @@
         Completely delete all artifacts and aliases of the given artifact name.
         This operation is irreversible. It will remove all related S3 artifacts
         and DynamoDB items.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        s3path = self._get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
+        s3path = self.get_artifact_s3path(name=name, version=constants.LATEST_VERSION)
         s3dir = s3path.parent
         s3dir.delete(bsm=bsm)
 
-        Artifact = self._get_artifact_class(bsm)
-        Alias = self._get_alias_class(bsm)
+        Artifact = self._artifact_class
+        Alias = self._alias_class
         with Artifact.batch_write() as batch:
             for artifact in Artifact.query(hash_key=name):
                 batch.delete(artifact)
         with Alias.batch_write() as batch:
             for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name)):
                 batch.delete(alias)
```

### Comparing `versioned-0.3.1/versioned/dynamodb.py` & `versioned-0.3.2/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/versioned/paths.py` & `versioned-0.3.2/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/versioned/tests/mock_aws.py` & `versioned-0.3.2/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/versioned/vendor/hashes.py` & `versioned-0.3.2/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/versioned/vendor/pytest_cov_helper.py` & `versioned-0.3.2/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.3.1/versioned.egg-info/PKG-INFO` & `versioned-0.3.2/versioned.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.3.1
+Version: 0.3.2
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.3.1/versioned.egg-info/SOURCES.txt` & `versioned-0.3.2/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

