# Comparing `tmp/versioned-0.2.1.tar.gz` & `tmp/versioned-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.2.1.tar", last modified: Thu Jul  6 03:04:37 2023, max compression
+gzip compressed data, was "versioned-0.3.1.tar", last modified: Thu Jul  6 15:40:41 2023, max compression
```

## Comparing `versioned-0.2.1.tar` & `versioned-0.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.306188 versioned-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 03:04:37.306025 versioned-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.2.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1989 2023-07-06 03:03:13.000000 versioned-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.2.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 03:04:37.306244 versioned-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.301746 versioned-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      928 2023-07-02 18:12:33.000000 versioned-0.2.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9730 2023-07-06 03:01:37.000000 versioned-0.2.1/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.303794 versioned-0.2.1/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.2.1/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 03:01:44.000000 versioned-0.2.1/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      681 2023-07-02 15:34:12.000000 versioned-0.2.1/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2037 2023-07-02 06:41:57.000000 versioned-0.2.1/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.2.1/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13868 2023-07-06 02:57:01.000000 versioned-0.2.1/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.304583 versioned-0.2.1/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.2.1/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.2.1/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.305058 versioned-0.2.1/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.2.1/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.305735 versioned-0.2.1/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.2.1/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.304455 versioned-0.2.1/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.104995 versioned-0.3.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.3.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.3.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.3.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 15:40:41.104871 versioned-0.3.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.3.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2848 2023-07-06 15:33:50.000000 versioned-0.3.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.3.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.3.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.3.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.3.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.3.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 15:40:41.105032 versioned-0.3.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.3.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.100741 versioned-0.3.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1039 2023-07-06 15:32:11.000000 versioned-0.3.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    10000 2023-07-06 15:23:09.000000 versioned-0.3.1/tests/test_core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.102893 versioned-0.3.1/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.3.1/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 15:35:28.000000 versioned-0.3.1/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      330 2023-07-06 15:30:51.000000 versioned-0.3.1/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1945 2023-07-06 15:24:44.000000 versioned-0.3.1/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.3.1/versioned/constants.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    16712 2023-07-06 15:21:05.000000 versioned-0.3.1/versioned/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.103587 versioned-0.3.1/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.3.1/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.3.1/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.103978 versioned-0.3.1/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.3.1/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.104687 versioned-0.3.1/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.3.1/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.3.1/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 15:40:41.103481 versioned-0.3.1/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 15:40:41.000000 versioned-0.3.1/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.2.1/AUTHORS.rst` & `versioned-0.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/LICENSE.txt` & `versioned-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/PKG-INFO` & `versioned-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.2.1
+Version: 0.3.1
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.2.1/README.rst` & `versioned-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/release-history.rst` & `versioned-0.3.1/release-history.rst`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,32 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.1 (2023-07-06)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Created a new public API class ``versioned.api.Repository``, allow developer to customize the S3 bucket and DynamoDB table name backend. So old API are renamed to:
+    - ``versioned.api.Repository.bootstrap``
+    - ``versioned.api.Repository.put_artifact``
+    - ``versioned.api.Repository.get_artifact_version``
+    - ``versioned.api.Repository.list_artifact_versions``
+    - ``versioned.api.Repository.publish_artifact_version``
+    - ``versioned.api.Repository.delete_artifact_version``
+    - ``versioned.api.Repository.put_alias``
+    - ``versioned.api.Repository.get_alias``
+    - ``versioned.api.Repository.list_aliases``
+    - ``versioned.api.Repository.delete_alias``
+    - ``versioned.api.Repository.purge_artifact``
+
+
 0.2.1 (2023-07-05)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``content_type``, ``metadata``, ``tags`` arguments to ``versioned.put_artifact``.
 - ``versioned.put_artifact`` now will skip uploading to s3 if ``content`` is not changed.
```

### Comparing `versioned-0.2.1/requirements-doc.txt` & `versioned-0.3.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/setup.py` & `versioned-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/tests/test_core.py` & `versioned-0.3.1/tests/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,211 +6,203 @@
 from s3pathlib import S3Path, context
 
 from versioned import exc
 from versioned import constants
 from versioned.bootstrap import bootstrap
 from versioned.dynamodb import encode_version
 from versioned.tests.mock_aws import BaseMockTest
-from versioned.core import (
-    put_artifact,
-    list_artifact_versions,
-    get_artifact_version,
-    publish_artifact_version,
-    delete_artifact_version,
-    put_alias,
-    get_alias,
-    list_aliases,
-    delete_alias,
-    purge_artifact,
-)
+from versioned.core import Repository
 
 from rich import print as rprint
 
 
 class Test(BaseMockTest):
     use_mock = True
 
     mock_list = [
         moto.mock_sts,
         moto.mock_s3,
         moto.mock_dynamodb,
     ]
 
+    repo: Repository = None
+
     @classmethod
     def setup_class_post_hook(cls):
         context.attach_boto_session(cls.bsm.boto_ses)
-        bootstrap(cls.bsm)
+        cls.repo = Repository()
+        cls.repo.bootstrap(cls.bsm)
 
     def _test(self):
         name = "deploy"
         alias = "LIVE"
 
-        purge_artifact(bsm=self.bsm, name=name)
+        self.repo.purge_artifact(bsm=self.bsm, name=name)
 
         # ======================================================================
         # Artifact
         # ======================================================================
         # --- test ArtifactNotFoundError ---
         # at this moment, no artifact exists
         with pytest.raises(exc.ArtifactNotFoundError):
-            publish_artifact_version(bsm=self.bsm, name=name)
+            self.repo.publish_artifact_version(bsm=self.bsm, name=name)
 
         with pytest.raises(exc.ArtifactNotFoundError):
-            get_artifact_version(bsm=self.bsm, name=name)
+            self.repo.get_artifact_version(bsm=self.bsm, name=name)
 
-        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
+        artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
 
         # put artifact
-        artifact = put_artifact(
+        artifact = self.repo.put_artifact(
             bsm=self.bsm,
             name=name,
             content=b"v1",
             content_type="text/plain",
             metadata={"foo": "bar"},
         )
         # rprint(artifact)
         # put artifact with the same content, S3 and Dynamodb should not changed
-        artifact = put_artifact(bsm=self.bsm, name=name, content=b"v1")
+        artifact = self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v1")
 
         def _assert_artifact(artifact):
             assert artifact.name == name
             assert artifact.version == constants.LATEST_VERSION
             assert artifact.s3uri.endswith(constants.LATEST_VERSION)
             assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         _assert_artifact(artifact)
 
-        artifact = get_artifact_version(bsm=self.bsm, name=name)
+        artifact = self.repo.get_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         _assert_artifact(artifact)
 
-        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
+        artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         # rprint(artifact_list)
         assert len(artifact_list) == 1
         _assert_artifact(artifact_list[0])
 
-        artifact = publish_artifact_version(bsm=self.bsm, name=name)
+        artifact = self.repo.publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "1"
         assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL))
         assert artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL)
         assert artifact.s3path.metadata["foo"] == "bar"
         assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         # put artifact again
-        artifact = put_artifact(bsm=self.bsm, name=name, content=b"v2")
+        artifact = self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v2")
         # rprint(artifact)
         assert artifact.version == constants.LATEST_VERSION
         assert S3Path(artifact.s3uri).read_text(bsm=self.bsm) == "v2"
 
-        artifact = publish_artifact_version(bsm=self.bsm, name=name)
+        artifact = self.repo.publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "2"
         s3path = S3Path(artifact.s3uri)
         assert artifact.s3uri.endswith("2".zfill(constants.VERSION_ZFILL))
         assert artifact.s3path.basename == str("2").zfill(constants.VERSION_ZFILL)
         assert artifact.get_content(bsm=self.bsm) == b"v2"
 
-        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
+        artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 3
 
         # ======================================================================
         # Artifact
         # ======================================================================
         # --- test raises error ---
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
-            put_alias(bsm=self.bsm, name=name, alias=alias, version=999)
+            self.repo.put_alias(bsm=self.bsm, name=name, alias=alias, version=999)
 
         # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
-            put_alias(bsm=self.bsm, name=name, alias=alias, secondary_version=999)
+            self.repo.put_alias(bsm=self.bsm, name=name, alias=alias, secondary_version=999)
 
         # secondary_version_weight type is wrong
         with pytest.raises(TypeError):
-            put_alias(
+            self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 secondary_version=999,
                 secondary_version_weight=0.5,
             )
 
         # secondary_version_weight value range is wrong
         with pytest.raises(ValueError):
-            put_alias(
+            self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 secondary_version=999,
                 secondary_version_weight=-100,
             )
 
         # secondary_version_weight value range is wrong
         with pytest.raises(ValueError):
-            put_alias(
+            self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 secondary_version=999,
                 secondary_version_weight=999,
             )
 
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
-            put_alias(
+            self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 secondary_version=999,
                 secondary_version_weight=20,
             )
 
         # version and secondary_version is the same
         with pytest.raises(ValueError):
-            put_alias(
+            self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 version=1,
                 secondary_version=1,
                 secondary_version_weight=20,
             )
 
         # alias not exists
         with pytest.raises(exc.AliasNotFoundError):
-            get_alias(bsm=self.bsm, name=name, alias="Invalid")
+            self.repo.get_alias(bsm=self.bsm, name=name, alias="Invalid")
 
         # put alias
-        ali = put_alias(bsm=self.bsm, name=name, alias=alias)
+        ali = self.repo.put_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
 
         def _assert_alias(ali):
             assert ali.name == name
             assert ali.alias == alias
             assert ali.version == constants.LATEST_VERSION
             assert ali.secondary_version is None
             assert ali.secondary_version_weight is None
             assert ali.version_s3uri.endswith(constants.LATEST_VERSION)
             assert ali.secondary_version_s3uri is None
             assert ali.get_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
-        ali = get_alias(bsm=self.bsm, name=name, alias=alias)
+        ali = self.repo.get_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
         _assert_alias(ali)
 
-        ali_list = list_aliases(bsm=self.bsm, name=name)
+        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 1
         _assert_alias(ali_list[0])
 
         # put alias again
-        ali = put_alias(
+        ali = self.repo.put_alias(
             bsm=self.bsm,
             name=name,
             alias=alias,
             version=1,
             secondary_version=2,
             secondary_version_weight=20,
         )
@@ -225,57 +217,57 @@
             assert ali.version_s3uri.endswith(encode_version(1))
             assert ali.secondary_version_s3uri.endswith(encode_version(2))
             assert ali.get_version_content(bsm=self.bsm) == b"v1"
             assert ali.get_secondary_version_content(bsm=self.bsm) == b"v2"
 
         _assert_alias(ali)
 
-        ali = get_alias(bsm=self.bsm, name=name, alias=alias)
+        ali = self.repo.get_alias(bsm=self.bsm, name=name, alias=alias)
         # rprint(ali)
         _assert_alias(ali)
 
-        ali_list = list_aliases(bsm=self.bsm, name=name)
+        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 1
         _assert_alias(ali_list[0])
 
         # --- test delete methods
-        delete_alias(bsm=self.bsm, name=name, alias=alias)
+        self.repo.delete_alias(bsm=self.bsm, name=name, alias=alias)
         with pytest.raises(exc.AliasNotFoundError):
-            get_alias(bsm=self.bsm, name=name, alias=alias)
-        ali_list = list_aliases(bsm=self.bsm, name=name)
+            self.repo.get_alias(bsm=self.bsm, name=name, alias=alias)
+        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 0
 
-        delete_artifact_version(bsm=self.bsm, name=name)
+        self.repo.delete_artifact_version(bsm=self.bsm, name=name)
         with pytest.raises(exc.ArtifactNotFoundError):
-            get_artifact_version(bsm=self.bsm, name=name)
-        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
+            self.repo.get_artifact_version(bsm=self.bsm, name=name)
+        artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 2
 
-        delete_artifact_version(bsm=self.bsm, name=name, version=1)
+        self.repo.delete_artifact_version(bsm=self.bsm, name=name, version=1)
         with pytest.raises(exc.ArtifactNotFoundError):
-            get_artifact_version(bsm=self.bsm, name=name, version=1)
-        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
+            self.repo.get_artifact_version(bsm=self.bsm, name=name, version=1)
+        artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 1
 
         # it is a soft delete, so S3 artifact is not deleted
         assert s3path.parent.count_objects(bsm=self.bsm) == 3
 
         # --- purge
         with pytest.raises(exc.ArtifactNotFoundError):
-            put_alias(bsm=self.bsm, name=name, alias="DEV", version=1)
+            self.repo.put_alias(bsm=self.bsm, name=name, alias="DEV", version=1)
 
-        put_alias(bsm=self.bsm, name=name, alias="DEV", version=2)
-        ali_list = list_aliases(bsm=self.bsm, name=name)
+        self.repo.put_alias(bsm=self.bsm, name=name, alias="DEV", version=2)
+        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 1
 
-        purge_artifact(bsm=self.bsm, name=name)
+        self.repo.purge_artifact(bsm=self.bsm, name=name)
         assert s3path.parent.count_objects(bsm=self.bsm) == 0
-        artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
+        artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
-        ali_list = list_aliases(bsm=self.bsm, name=name)
+        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 0
 
     def test(self):
         self._test()
 
 
 if __name__ == "__main__":
```

### Comparing `versioned-0.2.1/versioned/bootstrap.py` & `versioned-0.3.1/versioned/bootstrap.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 """
 
 import typing as T
 from boto_session_manager import BotoSesManager
 
 from pynamodb.models import PAY_PER_REQUEST_BILLING_MODE
 from pynamodb.connection import Connection
-from . import constants
 from . import dynamodb
 
 
 def bootstrap(
     bsm: BotoSesManager,
+    bucket_name: str,
+    dynamodb_table_name: str,
     dynamodb_write_capacity_units: T.Optional[int] = None,
     dynamodb_read_capacity_units: T.Optional[int] = None,
-    skip_s3: bool = False,
-    skip_dynamodb: bool = False,
 ):
     """
     Bootstrap the associated AWS account and region in the boto session manager.
     Create the S3 bucket and DynamoDB table if not exist.
     """
     # validate input arguments
     if sum(
@@ -36,36 +35,38 @@
     ]:  # pragma: no cover
         raise ValueError
 
     aws_account_id = bsm.sts_client.get_caller_identity()["Account"]
     aws_region = bsm.aws_region
 
     # create s3 bucket
-    if skip_s3 is False:
-        bucket = f"{aws_account_id}-{aws_region}-{constants.BUCKET_NAME}"
-        bsm.s3_client.create_bucket(Bucket=bucket)
+    try:
+        bsm.s3_client.head_bucket(Bucket=bucket_name)
+    except Exception as e:
+        if "Not Found" in str(e):
+            bsm.s3_client.create_bucket(Bucket=bucket_name)
+        else:
+            raise e
 
     # create dynamodb table
-    if skip_dynamodb is False:
-        if (
-            dynamodb_write_capacity_units is None
-            and dynamodb_read_capacity_units is None
-        ):
-
-            class Base(dynamodb.Base):
-                class Meta:
-                    table_name = constants.DYNAMODB_TABLE_NAME
-                    region = aws_region
-                    billing_mode = PAY_PER_REQUEST_BILLING_MODE
-
-        else:  # pragma: no cover
-
-            class Base(dynamodb.Base):
-                class Meta:
-                    table_name = constants.DYNAMODB_TABLE_NAME
-                    region = aws_region
-                    write_capacity_units = dynamodb_write_capacity_units
-                    read_capacity_units = dynamodb_read_capacity_units
-
-        with bsm.awscli():
-            Connection()
-            Base.create_table(wait=True)
+    if (
+        dynamodb_write_capacity_units is None
+        and dynamodb_read_capacity_units is None
+    ):
+        class Base(dynamodb.Base):
+            class Meta:
+                table_name = dynamodb_table_name
+                region = aws_region
+                billing_mode = PAY_PER_REQUEST_BILLING_MODE
+
+    else:  # pragma: no cover
+
+        class Base(dynamodb.Base):
+            class Meta:
+                table_name = dynamodb_table_name
+                region = aws_region
+                write_capacity_units = dynamodb_write_capacity_units
+                read_capacity_units = dynamodb_read_capacity_units
+
+    with bsm.awscli():
+        Connection()
+        Base.create_table(wait=True)
```

### Comparing `versioned-0.2.1/versioned/core.py` & `versioned-0.3.1/versioned/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 from boto_session_manager import BotoSesManager
 from s3pathlib import S3Path
 from func_args import NOTHING
 
 from . import constants
 from . import dynamodb
 from . import exc
+from .bootstrap import bootstrap
 from .vendor.hashes import hashes
 
 hashes.use_sha256()
 
 
 @dataclasses.dataclass
 class Artifact:
     """
     Data class for artifact.
 
+    It is not the same as the underlying DynamodbItem, it is a public facing
+    API data class.
+
     :param name: artifact name.
     :param version: artifact version.
     :param update_at: a utc datetime object, when this artifact was updated.
     :param s3uri: s3uri of the artifact version.
     :param sha256: sha256 of the content of the artifact version.
     """
 
@@ -50,14 +54,17 @@
 
 
 @dataclasses.dataclass
 class Alias:
     """
     Data class for alias.
 
+    It is not the same as the underlying DynamodbItem, it is a public facing
+    API data class.
+
     :param name: artifact name.
     :param alias: alias name. alias name cannot have hyphen
     :param version: artifact version. If ``None``, the latest version is used.
     :param secondary_version: see above.
     :param secondary_version_weight: an integer between 0 ~ 100.
     :param version_s3uri: s3uri of the primary artifact version of this alias.
     :param secondary_version_s3uri: s3uri of the secondary artifact version of this alias.
@@ -94,367 +101,399 @@
     def get_secondary_version_content(self, bsm: BotoSesManager) -> bytes:
         """
         Get the content of the secondary artifact version of this alias.
         """
         return self.s3path_secondary_version.read_bytes(bsm=bsm)
 
 
-def _get_artifact_class(bsm: BotoSesManager) -> T.Type[dynamodb.Artifact]:
-    class Artifact(dynamodb.Artifact):
-        class Meta:
-            table_name = constants.DYNAMODB_TABLE_NAME
-            region = bsm.aws_region
-
-    return Artifact
-
-
-def _get_alias_class(bsm: BotoSesManager) -> T.Type[dynamodb.Alias]:
-    class Alias(dynamodb.Alias):
-        class Meta:
-            table_name = constants.DYNAMODB_TABLE_NAME
-            region = bsm.aws_region
-
-    return Alias
-
-
-def _get_bucket(bsm: BotoSesManager) -> str:
-    return f"{bsm.aws_account_id}-{bsm.aws_region}-{constants.BUCKET_NAME}"
-
-
-def _get_s3path(bsm: BotoSesManager, name: str, version: str) -> S3Path:
-    return S3Path(_get_bucket(bsm=bsm)).joinpath(
-        constants.S3_PREFIX,
-        name,
-        dynamodb.encode_version(version),
+@dataclasses.dataclass
+class Repository:
+    s3_bucket: T.Optional[str] = dataclasses.field(default=None)
+    s3_prefix: T.Optional[str] = dataclasses.field(default=constants.S3_PREFIX)
+    dynamodb_table_name: T.Optional[str] = dataclasses.field(
+        default=constants.DYNAMODB_TABLE_NAME
     )
 
+    def _get_s3_bucket(self, bsm: BotoSesManager) -> str:
+        if self.s3_bucket is None:
+            return f"{bsm.aws_account_id}-{bsm.aws_region}-{constants.BUCKET_NAME}"
+        else:
+            return self.s3_bucket
+
+    def _get_s3path(self, bsm: BotoSesManager, name: str, version: str) -> S3Path:
+        return S3Path(self._get_s3_bucket(bsm=bsm)).joinpath(
+            self.s3_prefix,
+            name,
+            dynamodb.encode_version(version),
+        )
 
-def _get_artifact_dict(
-    bsm: BotoSesManager,
-    artifact: dynamodb.Artifact,
-) -> Artifact:
-    dct = artifact.to_dict()
-    dct["s3uri"] = _get_s3path(
-        bsm=bsm,
-        name=artifact.name,
-        version=artifact.version,
-    ).uri
-    return Artifact(**dct)
-
-
-def _get_alias_dict(
-    bsm: BotoSesManager,
-    alias: dynamodb.Alias,
-) -> Alias:
-    dct = alias.to_dict()
-    dct["version_s3uri"] = _get_s3path(
-        bsm=bsm,
-        name=alias.name,
-        version=alias.version,
-    ).uri
-    if alias.secondary_version is None:
-        dct["secondary_version_s3uri"] = None
-    else:
-        dct["secondary_version_s3uri"] = _get_s3path(
+    def bootstrap(
+        self,
+        bsm: BotoSesManager,
+        dynamodb_write_capacity_units: T.Optional[int] = None,
+        dynamodb_read_capacity_units: T.Optional[int] = None,
+    ):
+        bootstrap(
             bsm=bsm,
-            name=alias.name,
-            version=alias.secondary_version,
-        ).uri
-    return Alias(**dct)
-
-
-# ------------------------------------------------------------------------------
-# Artifact
-# ------------------------------------------------------------------------------
-def put_artifact(
-    bsm: BotoSesManager,
-    name: str,
-    content: bytes,
-    content_type: str = NOTHING,
-    metadata: T.Dict[str, str] = NOTHING,
-    tags: T.Dict[str, str] = NOTHING,
-) -> Artifact:
-    """
-    Create / Update artifact to the latest.
-
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    :param content: binary artifact content.
-    :param metadata: optional metadata of the s3 object.
-    :param tags: optional tags of the s3 object.
-    """
-    Artifact = _get_artifact_class(bsm)
-    artifact = Artifact.new(name=name)
-    artifact_sha256 = hashes.of_bytes(content)
-    artifact.sha256 = artifact_sha256
-    s3path = _get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
-
-    # do nothing if the content is not changed
-    if s3path.exists(bsm=bsm):
-        if s3path.metadata["artifact_sha256"] == artifact_sha256:
-            return _get_artifact_dict(bsm=bsm, artifact=artifact)
-
-    final_metadata = dict(
-        artifact_name=name,
-        artifact_sha256=artifact_sha256,
-    )
-    if metadata is not NOTHING:
-        final_metadata.update(metadata)
-    s3path.write_bytes(
-        content,
-        metadata=final_metadata,
-        content_type=content_type,
-        tags=tags,
-        bsm=bsm,
-    )
-    artifact.save()
-    return _get_artifact_dict(bsm=bsm, artifact=artifact)
-
-
-def _get_artifact_dynamodb_item(
-    artifact_class: T.Type[dynamodb.Artifact],
-    name: str,
-    version: T.Union[int, str],
-) -> dynamodb.Artifact:
-    try:
-        artifact = artifact_class.get(
-            hash_key=name,
-            range_key=dynamodb.encode_version(version),
+            bucket_name=self._get_s3_bucket(bsm=bsm),
+            dynamodb_table_name=self.dynamodb_table_name,
+            dynamodb_write_capacity_units=dynamodb_write_capacity_units,
+            dynamodb_read_capacity_units=dynamodb_read_capacity_units,
         )
-        if artifact.is_deleted:
-            raise exc.ArtifactNotFoundError(f"name = {name!r}, version = {version!r}")
-        return artifact
-    except artifact_class.DoesNotExist:
-        raise exc.ArtifactNotFoundError(f"name = {name!r}, version = {version!r}")
-
-
-def get_artifact_version(
-    bsm: BotoSesManager,
-    name: str,
-    version: T.Optional[T.Union[int, str]] = None,
-) -> Artifact:
-    """
-    Return the information about the artifact or artifact version.
 
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    :param version: artifact version. If ``None``, return the latest version.
-    """
-    Artifact = _get_artifact_class(bsm)
-    if version is None:
-        version = constants.LATEST_VERSION
-    artifact = _get_artifact_dynamodb_item(Artifact, name=name, version=version)
-    return _get_artifact_dict(bsm=bsm, artifact=artifact)
-
-
-def list_artifact_versions(
-    bsm: BotoSesManager,
-    name: str,
-) -> T.List[Artifact]:
-    """
-    Return a list of artifact versions. The latest version is always the first item.
-    And the newer version comes first.
+    def _get_artifact_class(self, bsm: BotoSesManager) -> T.Type[dynamodb.Artifact]:
+        class Artifact(dynamodb.Artifact):
+            class Meta:
+                table_name = self.dynamodb_table_name
+                region = bsm.aws_region
+
+        return Artifact
+
+    def _get_alias_class(self, bsm: BotoSesManager) -> T.Type[dynamodb.Alias]:
+        class Alias(dynamodb.Alias):
+            class Meta:
+                table_name = self.dynamodb_table_name
+                region = bsm.aws_region
+
+        return Alias
+
+    def _get_artifact_object(
+        self,
+        bsm: BotoSesManager,
+        artifact: dynamodb.Artifact,
+    ) -> Artifact:
+        dct = artifact.to_dict()
+        dct["s3uri"] = self._get_s3path(
+            bsm=bsm,
+            name=artifact.name,
+            version=artifact.version,
+        ).uri
+        return Artifact(**dct)
 
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    """
-    Artifact = _get_artifact_class(bsm)
-    return [
-        _get_artifact_dict(bsm=bsm, artifact=artifact)
-        for artifact in Artifact.query(
-            hash_key=name,
-            scan_index_forward=False,
-            filter_condition=Artifact.is_deleted == False,
+    def _get_alias_object(
+        self,
+        bsm: BotoSesManager,
+        alias: dynamodb.Alias,
+    ) -> Alias:
+        dct = alias.to_dict()
+        dct["version_s3uri"] = self._get_s3path(
+            bsm=bsm,
+            name=alias.name,
+            version=alias.version,
+        ).uri
+        if alias.secondary_version is None:
+            dct["secondary_version_s3uri"] = None
+        else:
+            dct["secondary_version_s3uri"] = self._get_s3path(
+                bsm=bsm,
+                name=alias.name,
+                version=alias.secondary_version,
+            ).uri
+        return Alias(**dct)
+
+    # ------------------------------------------------------------------------------
+    # Artifact
+    # ------------------------------------------------------------------------------
+    def put_artifact(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        content: bytes,
+        content_type: str = NOTHING,
+        metadata: T.Dict[str, str] = NOTHING,
+        tags: T.Dict[str, str] = NOTHING,
+    ) -> Artifact:
+        """
+        Create / Update artifact to the latest.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        :param content: binary artifact content.
+        :param metadata: optional metadata of the s3 object.
+        :param tags: optional tags of the s3 object.
+        """
+        Artifact = self._get_artifact_class(bsm)
+        artifact = Artifact.new(name=name)
+        artifact_sha256 = hashes.of_bytes(content)
+        artifact.sha256 = artifact_sha256
+        s3path = self._get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
+
+        # do nothing if the content is not changed
+        if s3path.exists(bsm=bsm):
+            if s3path.metadata["artifact_sha256"] == artifact_sha256:
+                return self._get_artifact_object(bsm=bsm, artifact=artifact)
+
+        final_metadata = dict(
+            artifact_name=name,
+            artifact_sha256=artifact_sha256,
         )
-    ]
-
-
-def publish_artifact_version(
-    bsm: BotoSesManager,
-    name: str,
-) -> Artifact:
-    """
-    Creates a version from the latest artifact. Use versions to create an
-    immutable snapshot of your latest artifact.
-
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    """
-    Artifact = _get_artifact_class(bsm)
-    artifacts = list(Artifact.query(hash_key=name, scan_index_forward=False, limit=2))
-    if len(artifacts) == 0:
-        raise exc.ArtifactNotFoundError(f"name = {name!r}")
-    elif len(artifacts) == 1:
-        new_version = "1"
-    else:
-        new_version = str(int(artifacts[1].version) + 1)
-    artifact = Artifact.new(name=name, version=new_version)
-    artifact.sha256 = artifacts[0].sha256
-    artifact.save()
-    s3path_old = _get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
-    s3path_new = _get_s3path(bsm=bsm, name=name, version=new_version)
-    s3path_old.copy_to(s3path_new, bsm=bsm)
-    return _get_artifact_dict(bsm=bsm, artifact=artifact)
-
-
-def delete_artifact_version(
-    bsm: BotoSesManager,
-    name: str,
-    version: T.Optional[T.Union[int, str]] = None,
-):
-    """
-    Deletes a specific version of artifact. If version is not specified,
-    the latest version is deleted. Note that this is a soft delete,
-    neither the S3 artifact nor the DynamoDB item is deleted. It is just
-    become "invisible" to the :func:`get_artifact` and :func:`list_artifacts``.
-
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    :param version: artifact version. If ``None``, delete the latest version.
-    """
-    Artifact = _get_artifact_class(bsm)
-    if version is None:
-        version = constants.LATEST_VERSION
-    res = Artifact.new(name=name, version=version).update(
-        actions=[
-            Artifact.is_deleted.set(True),
-        ],
-    )
-    # print(res)
-
-
-# ------------------------------------------------------------------------------
-# Alias
-# ------------------------------------------------------------------------------
-def put_alias(
-    bsm: BotoSesManager,
-    name: str,
-    alias: str,
-    version: T.Optional[T.Union[int, str]] = None,
-    secondary_version: T.Optional[T.Union[int, str]] = None,
-    secondary_version_weight: T.Optional[int] = None,
-) -> Alias:
-    """
-    Creates an alias for an artifact version. If ``version`` is not specified,
-    the latest version is used.
-
-    You can also map an alias to split invocation requests between two versions.
-    Use the ``secondary_version`` and ``secondary_version_weight`` to specify
-    a second version and the percentage of invocation requests that it receives.
-
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    :param alias: alias name. alias name cannot have hyphen
-    :param version: artifact version. If ``None``, the latest version is used.
-    :param secondary_version: see above.
-    :param secondary_version_weight: an integer between 0 ~ 100.
-    """
-    # validate argument
-    if "-" in alias:  # pragma: no cover
-        raise ValueError("alias cannot have hyphen")
-
-    if secondary_version is not None:
-        if not isinstance(secondary_version_weight, int):
-            raise TypeError("secondary_version_weight must be int")
-        if not (0 <= secondary_version_weight < 100):
-            raise ValueError("secondary_version_weight must be 0 <= x < 100")
-
-    # ensure the artifact exists
-    Artifact = _get_artifact_class(bsm)
-    if version is None:
-        version = constants.LATEST_VERSION
-    _get_artifact_dynamodb_item(Artifact, name=name, version=version)
-    if secondary_version is not None:
-        _get_artifact_dynamodb_item(Artifact, name=name, version=secondary_version)
-
-    Alias = _get_alias_class(bsm)
-    alias = Alias.new(
-        name=name,
-        alias=alias,
-        version=version,
-        secondary_version=secondary_version,
-        secondary_version_weight=secondary_version_weight,
-    )
-
-    alias.save()
-    return _get_alias_dict(bsm=bsm, alias=alias)
-
-
-def get_alias(
-    bsm: BotoSesManager,
-    name: str,
-    alias: str,
-) -> Alias:
-    """
-    Return details about the alias.
-
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    :param alias: alias name. alias name cannot have hyphen
-    """
-    Alias = _get_alias_class(bsm)
-    try:
-        return _get_alias_dict(
+        if metadata is not NOTHING:
+            final_metadata.update(metadata)
+        s3path.write_bytes(
+            content,
+            metadata=final_metadata,
+            content_type=content_type,
+            tags=tags,
             bsm=bsm,
-            alias=Alias.get(
-                hash_key=dynamodb.encode_alias_key(name),
-                range_key=alias,
-            ),
         )
-    except Alias.DoesNotExist:
-        raise exc.AliasNotFoundError(f"name = {name!r}, alias = {alias!r}")
-
+        artifact.save()
+        return self._get_artifact_object(bsm=bsm, artifact=artifact)
 
-def list_aliases(
-    bsm: BotoSesManager,
-    name: str,
-) -> T.List[Alias]:
-    """
-    Returns a list of aliases for an artifact.
-
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    """
-    Alias = _get_alias_class(bsm)
-    return [
-        _get_alias_dict(bsm=bsm, alias=alias)
-        for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name))
-    ]
+    def _get_artifact_dynamodb_item(
+        self,
+        artifact_class: T.Type[dynamodb.Artifact],
+        name: str,
+        version: T.Union[int, str],
+    ) -> dynamodb.Artifact:
+        try:
+            artifact = artifact_class.get(
+                hash_key=name,
+                range_key=dynamodb.encode_version(version),
+            )
+            if artifact.is_deleted:
+                raise exc.ArtifactNotFoundError(
+                    f"name = {name!r}, version = {version!r}"
+                )
+            return artifact
+        except artifact_class.DoesNotExist:
+            raise exc.ArtifactNotFoundError(f"name = {name!r}, version = {version!r}")
 
+    def get_artifact_version(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        version: T.Optional[T.Union[int, str]] = None,
+    ) -> Artifact:
+        """
+        Return the information about the artifact or artifact version.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        :param version: artifact version. If ``None``, return the latest version.
+        """
+        Artifact = self._get_artifact_class(bsm)
+        if version is None:
+            version = constants.LATEST_VERSION
+        artifact = self._get_artifact_dynamodb_item(
+            Artifact, name=name, version=version
+        )
+        return self._get_artifact_object(bsm=bsm, artifact=artifact)
 
-def delete_alias(
-    bsm: BotoSesManager,
-    name: str,
-    alias: str,
-):
-    """
-    Deletes an alias.
-    """
-    Alias = _get_alias_class(bsm)
-    res = Alias.new(name=name, alias=alias).delete()
-    # print(res)
+    def list_artifact_versions(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+    ) -> T.List[Artifact]:
+        """
+        Return a list of artifact versions. The latest version is always the first item.
+        And the newer version comes first.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        """
+        Artifact = self._get_artifact_class(bsm)
+        return [
+            self._get_artifact_object(bsm=bsm, artifact=artifact)
+            for artifact in Artifact.query(
+                hash_key=name,
+                scan_index_forward=False,
+                filter_condition=Artifact.is_deleted == False,
+            )
+        ]
+
+    def publish_artifact_version(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+    ) -> Artifact:
+        """
+        Creates a version from the latest artifact. Use versions to create an
+        immutable snapshot of your latest artifact.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        """
+        Artifact = self._get_artifact_class(bsm)
+        artifacts = list(
+            Artifact.query(hash_key=name, scan_index_forward=False, limit=2)
+        )
+        if len(artifacts) == 0:
+            raise exc.ArtifactNotFoundError(f"name = {name!r}")
+        elif len(artifacts) == 1:
+            new_version = "1"
+        else:
+            new_version = str(int(artifacts[1].version) + 1)
+        artifact = Artifact.new(name=name, version=new_version)
+        artifact.sha256 = artifacts[0].sha256
+        artifact.save()
+        s3path_old = self._get_s3path(
+            bsm=bsm, name=name, version=constants.LATEST_VERSION
+        )
+        s3path_new = self._get_s3path(bsm=bsm, name=name, version=new_version)
+        s3path_old.copy_to(s3path_new, bsm=bsm)
+        return self._get_artifact_object(bsm=bsm, artifact=artifact)
+
+    def delete_artifact_version(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        version: T.Optional[T.Union[int, str]] = None,
+    ):
+        """
+        Deletes a specific version of artifact. If version is not specified,
+        the latest version is deleted. Note that this is a soft delete,
+        neither the S3 artifact nor the DynamoDB item is deleted. It is just
+        become "invisible" to the :func:`get_artifact` and :func:`list_artifacts``.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        :param version: artifact version. If ``None``, delete the latest version.
+        """
+        Artifact = self._get_artifact_class(bsm)
+        if version is None:
+            version = constants.LATEST_VERSION
+        res = Artifact.new(name=name, version=version).update(
+            actions=[
+                Artifact.is_deleted.set(True),
+            ],
+        )
+        # print(res)
 
+    # ------------------------------------------------------------------------------
+    # Alias
+    # ------------------------------------------------------------------------------
+    def put_alias(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        alias: str,
+        version: T.Optional[T.Union[int, str]] = None,
+        secondary_version: T.Optional[T.Union[int, str]] = None,
+        secondary_version_weight: T.Optional[int] = None,
+    ) -> Alias:
+        """
+        Creates an alias for an artifact version. If ``version`` is not specified,
+        the latest version is used.
+
+        You can also map an alias to split invocation requests between two versions.
+        Use the ``secondary_version`` and ``secondary_version_weight`` to specify
+        a second version and the percentage of invocation requests that it receives.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        :param alias: alias name. alias name cannot have hyphen
+        :param version: artifact version. If ``None``, the latest version is used.
+        :param secondary_version: see above.
+        :param secondary_version_weight: an integer between 0 ~ 100.
+        """
+        # validate argument
+        if "-" in alias:  # pragma: no cover
+            raise ValueError("alias cannot have hyphen")
+
+        if secondary_version is not None:
+            if not isinstance(secondary_version_weight, int):
+                raise TypeError("secondary_version_weight must be int")
+            if not (0 <= secondary_version_weight < 100):
+                raise ValueError("secondary_version_weight must be 0 <= x < 100")
+
+        # ensure the artifact exists
+        Artifact = self._get_artifact_class(bsm)
+        if version is None:
+            version = constants.LATEST_VERSION
+        self._get_artifact_dynamodb_item(Artifact, name=name, version=version)
+        if secondary_version is not None:
+            self._get_artifact_dynamodb_item(
+                Artifact, name=name, version=secondary_version
+            )
+
+        Alias = self._get_alias_class(bsm)
+        alias = Alias.new(
+            name=name,
+            alias=alias,
+            version=version,
+            secondary_version=secondary_version,
+            secondary_version_weight=secondary_version_weight,
+        )
 
-def purge_artifact(
-    bsm: BotoSesManager,
-    name: str,
-):
-    """
-    Completely delete all artifacts and aliases of the given artifact name.
-    This operation is irreversible. It will remove all related S3 artifacts
-    and DynamoDB items.
+        alias.save()
+        return self._get_alias_object(bsm=bsm, alias=alias)
 
-    :param bsm: ``boto_session_manager.BotoSesManager`` object.
-    :param name: artifact name.
-    """
-    s3path = _get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
-    s3dir = s3path.parent
-    s3dir.delete(bsm=bsm)
-
-    Artifact = _get_artifact_class(bsm)
-    Alias = _get_alias_class(bsm)
-    with Artifact.batch_write() as batch:
-        for artifact in Artifact.query(hash_key=name):
-            batch.delete(artifact)
-    with Alias.batch_write() as batch:
-        for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name)):
-            batch.delete(alias)
+    def get_alias(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        alias: str,
+    ) -> Alias:
+        """
+        Return details about the alias.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        :param alias: alias name. alias name cannot have hyphen
+        """
+        Alias = self._get_alias_class(bsm)
+        try:
+            return self._get_alias_object(
+                bsm=bsm,
+                alias=Alias.get(
+                    hash_key=dynamodb.encode_alias_key(name),
+                    range_key=alias,
+                ),
+            )
+        except Alias.DoesNotExist:
+            raise exc.AliasNotFoundError(f"name = {name!r}, alias = {alias!r}")
+
+    def list_aliases(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+    ) -> T.List[Alias]:
+        """
+        Returns a list of aliases for an artifact.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        """
+        Alias = self._get_alias_class(bsm)
+        return [
+            self._get_alias_object(bsm=bsm, alias=alias)
+            for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name))
+        ]
+
+    def delete_alias(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        alias: str,
+    ):
+        """
+        Deletes an alias.
+        """
+        Alias = self._get_alias_class(bsm)
+        res = Alias.new(name=name, alias=alias).delete()
+        # print(res)
+
+    def purge_artifact(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+    ):
+        """
+        Completely delete all artifacts and aliases of the given artifact name.
+        This operation is irreversible. It will remove all related S3 artifacts
+        and DynamoDB items.
+
+        :param bsm: ``boto_session_manager.BotoSesManager`` object.
+        :param name: artifact name.
+        """
+        s3path = self._get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
+        s3dir = s3path.parent
+        s3dir.delete(bsm=bsm)
+
+        Artifact = self._get_artifact_class(bsm)
+        Alias = self._get_alias_class(bsm)
+        with Artifact.batch_write() as batch:
+            for artifact in Artifact.query(hash_key=name):
+                batch.delete(artifact)
+        with Alias.batch_write() as batch:
+            for alias in Alias.query(hash_key=dynamodb.encode_alias_key(name)):
+                batch.delete(alias)
```

### Comparing `versioned-0.2.1/versioned/dynamodb.py` & `versioned-0.3.1/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/versioned/paths.py` & `versioned-0.3.1/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/versioned/tests/mock_aws.py` & `versioned-0.3.1/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/versioned/vendor/hashes.py` & `versioned-0.3.1/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/versioned/vendor/pytest_cov_helper.py` & `versioned-0.3.1/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.2.1/versioned.egg-info/PKG-INFO` & `versioned-0.3.1/versioned.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.2.1
+Version: 0.3.1
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.3.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.2.1/versioned.egg-info/SOURCES.txt` & `versioned-0.3.1/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

