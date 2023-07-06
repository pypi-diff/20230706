# Comparing `tmp/versioned-0.1.2.tar.gz` & `tmp/versioned-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.1.2.tar", last modified: Sun Jul  2 18:26:46 2023, max compression
+gzip compressed data, was "versioned-0.2.1.tar", last modified: Thu Jul  6 03:04:37 2023, max compression
```

## Comparing `versioned-0.1.2.tar` & `versioned-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.226823 versioned-0.1.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.1.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.1.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.1.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-02 18:26:46.226667 versioned-0.1.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.1.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1674 2023-07-02 18:13:48.000000 versioned-0.1.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.1.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.1.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.1.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.1.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.1.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-02 18:26:46.226866 versioned-0.1.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.1.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.222532 versioned-0.1.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      928 2023-07-02 18:12:33.000000 versioned-0.1.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9398 2023-07-02 18:13:00.000000 versioned-0.1.2/tests/test_core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.224549 versioned-0.1.2/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.1.2/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-02 18:24:06.000000 versioned-0.1.2/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      681 2023-07-02 15:34:12.000000 versioned-0.1.2/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2037 2023-07-02 06:41:57.000000 versioned-0.1.2/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.1.2/versioned/constants.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    13257 2023-07-02 18:12:10.000000 versioned-0.1.2/versioned/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.225291 versioned-0.1.2/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.1.2/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.1.2/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.225812 versioned-0.1.2/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.1.2/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.226455 versioned-0.1.2/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.1.2/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.1.2/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-02 18:26:46.225175 versioned-0.1.2/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-02 18:26:46.000000 versioned-0.1.2/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.306188 versioned-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 03:04:37.306025 versioned-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2613 2023-07-02 18:23:51.000000 versioned-0.2.1/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1989 2023-07-06 03:03:13.000000 versioned-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.2.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      112 2023-07-02 06:52:10.000000 versioned-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-06 03:04:37.306244 versioned-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.301746 versioned-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      928 2023-07-02 18:12:33.000000 versioned-0.2.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     9730 2023-07-06 03:01:37.000000 versioned-0.2.1/tests/test_core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.303794 versioned-0.2.1/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.2.1/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-06 03:01:44.000000 versioned-0.2.1/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      681 2023-07-02 15:34:12.000000 versioned-0.2.1/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2037 2023-07-02 06:41:57.000000 versioned-0.2.1/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      206 2023-07-02 06:40:39.000000 versioned-0.2.1/versioned/constants.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    13868 2023-07-06 02:57:01.000000 versioned-0.2.1/versioned/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.304583 versioned-0.2.1/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3664 2023-07-02 16:28:39.000000 versioned-0.2.1/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.2.1/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.305058 versioned-0.2.1/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.2.1/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.305735 versioned-0.2.1/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-07-02 03:37:35.000000 versioned-0.2.1/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.2.1/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-06 03:04:37.304455 versioned-0.2.1/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3748 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      771 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      231 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-06 03:04:37.000000 versioned-0.2.1/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.1.2/AUTHORS.rst` & `versioned-0.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/LICENSE.txt` & `versioned-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/PKG-INFO` & `versioned-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.1.2
+Version: 0.2.1
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.1.2/README.rst` & `versioned-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/requirements-doc.txt` & `versioned-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/setup.py` & `versioned-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/tests/test_api.py` & `versioned-0.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/tests/test_core.py` & `versioned-0.2.1/tests/test_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,16 +57,24 @@
         with pytest.raises(exc.ArtifactNotFoundError):
             get_artifact_version(bsm=self.bsm, name=name)
 
         artifact_list = list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
 
         # put artifact
-        artifact = put_artifact(bsm=self.bsm, name=name, content=b"v1")
+        artifact = put_artifact(
+            bsm=self.bsm,
+            name=name,
+            content=b"v1",
+            content_type="text/plain",
+            metadata={"foo": "bar"},
+        )
         # rprint(artifact)
+        # put artifact with the same content, S3 and Dynamodb should not changed
+        artifact = put_artifact(bsm=self.bsm, name=name, content=b"v1")
 
         def _assert_artifact(artifact):
             assert artifact.name == name
             assert artifact.version == constants.LATEST_VERSION
             assert artifact.s3uri.endswith(constants.LATEST_VERSION)
             assert artifact.get_content(bsm=self.bsm) == b"v1"
 
@@ -82,14 +90,15 @@
         _assert_artifact(artifact_list[0])
 
         artifact = publish_artifact_version(bsm=self.bsm, name=name)
         # rprint(artifact)
         assert artifact.version == "1"
         assert artifact.s3uri.endswith("1".zfill(constants.VERSION_ZFILL))
         assert artifact.s3path.basename == str("1").zfill(constants.VERSION_ZFILL)
+        assert artifact.s3path.metadata["foo"] == "bar"
         assert artifact.get_content(bsm=self.bsm) == b"v1"
 
         # put artifact again
         artifact = put_artifact(bsm=self.bsm, name=name, content=b"v2")
         # rprint(artifact)
         assert artifact.version == constants.LATEST_VERSION
         assert S3Path(artifact.s3uri).read_text(bsm=self.bsm) == "v2"
```

### Comparing `versioned-0.1.2/versioned/api.py` & `versioned-0.2.1/versioned/api.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned/bootstrap.py` & `versioned-0.2.1/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned/core.py` & `versioned-0.2.1/versioned/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing as T
 
 import dataclasses
 from datetime import datetime
 
 from boto_session_manager import BotoSesManager
 from s3pathlib import S3Path
+from func_args import NOTHING
 
 from . import constants
 from . import dynamodb
 from . import exc
 from .vendor.hashes import hashes
 
 hashes.use_sha256()
@@ -164,36 +165,52 @@
 # ------------------------------------------------------------------------------
 # Artifact
 # ------------------------------------------------------------------------------
 def put_artifact(
     bsm: BotoSesManager,
     name: str,
     content: bytes,
+    content_type: str = NOTHING,
+    metadata: T.Dict[str, str] = NOTHING,
+    tags: T.Dict[str, str] = NOTHING,
 ) -> Artifact:
     """
     Create / Update artifact to the latest.
 
     :param bsm: ``boto_session_manager.BotoSesManager`` object.
     :param name: artifact name.
     :param content: binary artifact content.
+    :param metadata: optional metadata of the s3 object.
+    :param tags: optional tags of the s3 object.
     """
     Artifact = _get_artifact_class(bsm)
     artifact = Artifact.new(name=name)
     artifact_sha256 = hashes.of_bytes(content)
     artifact.sha256 = artifact_sha256
-    artifact.save()
     s3path = _get_s3path(bsm=bsm, name=name, version=constants.LATEST_VERSION)
+
+    # do nothing if the content is not changed
+    if s3path.exists(bsm=bsm):
+        if s3path.metadata["artifact_sha256"] == artifact_sha256:
+            return _get_artifact_dict(bsm=bsm, artifact=artifact)
+
+    final_metadata = dict(
+        artifact_name=name,
+        artifact_sha256=artifact_sha256,
+    )
+    if metadata is not NOTHING:
+        final_metadata.update(metadata)
     s3path.write_bytes(
         content,
-        metadata=dict(
-            artifact_name=name,
-            artifact_sha256=artifact_sha256,
-        ),
+        metadata=final_metadata,
+        content_type=content_type,
+        tags=tags,
         bsm=bsm,
     )
+    artifact.save()
     return _get_artifact_dict(bsm=bsm, artifact=artifact)
 
 
 def _get_artifact_dynamodb_item(
     artifact_class: T.Type[dynamodb.Artifact],
     name: str,
     version: T.Union[int, str],
```

### Comparing `versioned-0.1.2/versioned/dynamodb.py` & `versioned-0.2.1/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned/paths.py` & `versioned-0.2.1/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned/tests/mock_aws.py` & `versioned-0.2.1/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned/vendor/hashes.py` & `versioned-0.2.1/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned/vendor/pytest_cov_helper.py` & `versioned-0.2.1/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.1.2/versioned.egg-info/PKG-INFO` & `versioned-0.2.1/versioned.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.1.2
+Version: 0.2.1
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.1.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `versioned-0.1.2/versioned.egg-info/SOURCES.txt` & `versioned-0.2.1/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

