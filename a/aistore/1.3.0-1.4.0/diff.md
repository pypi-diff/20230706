# Comparing `tmp/aistore-1.3.0.tar.gz` & `tmp/aistore-1.4.0.tar.gz`

## Comparing `aistore-1.3.0.tar` & `aistore-1.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/client.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/common_requirements
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/version.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/botocore.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/botocore_requirements
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/README.md
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/__init__.py
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/aisio.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/dataset.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/dev_requirements
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/utils.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/README.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/__init__.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/ais_source.py
--rw-r--r--   0        0        0    26977 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/bucket.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/client.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/cluster.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/const.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/dsort.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/dsort_types.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/errors.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/etl.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/etl_const.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/etl_templates.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/job.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/list_object_flag.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/namespace.py
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object_attributes.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object_iterator.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object_reader.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/request_client.py
--rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/types.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/utils.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_collection.py
--rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_group.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_names.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_range.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_template.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.3.0/LICENSE
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.3.0/.gitignore
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.3.0/README.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aistore-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aistore-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/client.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/common_requirements
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/version.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/botocore_patch/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/botocore_patch/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/botocore_patch/botocore.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/botocore_patch/botocore_requirements
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/pytorch/README.md
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/pytorch/__init__.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/pytorch/aisio.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/pytorch/dataset.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/pytorch/dev_requirements
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/pytorch/utils.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/README.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/ais_source.py
+-rw-r--r--   0        0        0    32585 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/bucket.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/client.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/cluster.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/const.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/dsort.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/dsort_types.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/errors.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/etl.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/etl_const.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/etl_templates.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/job.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/list_object_flag.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/namespace.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/object.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/object_attributes.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/object_iterator.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/object_reader.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/request_client.py
+-rw-r--r--   0        0        0    11317 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/types.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/utils.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/multiobj/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/multiobj/object_collection.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/multiobj/object_group.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/multiobj/object_names.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/multiobj/object_range.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.4.0/aistore/sdk/multiobj/object_template.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.4.0/LICENSE
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.4.0/.gitignore
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.4.0/README.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aistore-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aistore-1.4.0/PKG-INFO
```

### Comparing `aistore-1.3.0/aistore/botocore_patch/README.md` & `aistore-1.4.0/aistore/botocore_patch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/botocore_patch/botocore.py` & `aistore-1.4.0/aistore/botocore_patch/botocore.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/pytorch/README.md` & `aistore-1.4.0/aistore/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/pytorch/aisio.py` & `aistore-1.4.0/aistore/pytorch/aisio.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/pytorch/dataset.py` & `aistore-1.4.0/aistore/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/pytorch/utils.py` & `aistore-1.4.0/aistore/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/README.md` & `aistore-1.4.0/aistore/sdk/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/ais_source.py` & `aistore-1.4.0/aistore/sdk/ais_source.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/bucket.py` & `aistore-1.4.0/aistore/sdk/bucket.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 #
 # Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 #
 
 from __future__ import annotations  # pylint: disable=unused-variable
 
+import json
 import logging
 from pathlib import Path
+import time
 from typing import Dict, List, NewType, Iterable
 import requests
 
 from aistore.sdk.ais_source import AISSource
 from aistore.sdk.etl_const import DEFAULT_ETL_TIMEOUT
 from aistore.sdk.object_iterator import ObjectIterator
 from aistore.sdk.const import (
     ACT_COPY_BCK,
     ACT_CREATE_BCK,
     ACT_DESTROY_BCK,
     ACT_ETL_BCK,
     ACT_EVICT_REMOTE_BCK,
     ACT_LIST,
     ACT_MOVE_BCK,
+    ACT_SUMMARY_BCK,
+    HEADER_ACCEPT,
+    HEADER_BUCKET_PROPS,
+    HEADER_BUCKET_SUMM,
     HTTP_METHOD_DELETE,
     HTTP_METHOD_GET,
     HTTP_METHOD_HEAD,
     HTTP_METHOD_POST,
+    MSGPACK_CONTENT_TYPE,
     PROVIDER_AIS,
     QPARAM_BCK_TO,
+    QPARAM_COUNT_REMOTE_OBJS,
+    QPARAM_FLT_PRESENCE,
     QPARAM_KEEP_REMOTE,
     QPARAM_NAMESPACE,
     QPARAM_PROVIDER,
     URL_PATH_BUCKETS,
-    HEADER_ACCEPT,
-    MSGPACK_CONTENT_TYPE,
+    STATUS_ACCEPTED,
+    STATUS_OK,
 )
 
 from aistore.sdk.errors import (
     InvalidBckProvider,
     ErrBckAlreadyExists,
     ErrBckNotFound,
+    UnexpectedHTTPStatusCode,
 )
 from aistore.sdk.multiobj import ObjectGroup, ObjectRange
 from aistore.sdk.request_client import RequestClient
 from aistore.sdk.object import Object
 from aistore.sdk.types import (
     ActionMsg,
     BucketEntry,
     BucketList,
     BucketModel,
+    BsummCtrlMsg,
     Namespace,
     CopyBckMsg,
     TransformBckMsg,
     TCBckMsg,
     ListObjectsMsg,
 )
 from aistore.sdk.list_object_flag import ListObjectFlag
@@ -246,14 +257,137 @@
         return self.client.request(
             HTTP_METHOD_HEAD,
             path=f"{URL_PATH_BUCKETS}/{self.name}",
             params=self.qparam,
         ).headers
 
     # pylint: disable=too-many-arguments
+    def summary(
+        self,
+        uuid: str = "",
+        prefix: str = "",
+        fast: bool = True,
+        cached: bool = True,
+        present: bool = True,
+    ):
+        """
+        Returns bucket summary (starts xaction job and polls for results).
+
+        Args:
+            uuid (str): Identifier for the bucket summary. Defaults to an empty string.
+            prefix (str): Prefix for objects to be included in the bucket summary.
+                          Defaults to an empty string (all objects).
+            fast (bool): If True, performs and returns a quick summary. Defaults to True.
+            cached (bool): If True, summary entails cached entities. Defaults to True.
+            present (bool): If True, summary entails present entities. Defaults to True.
+
+        Raises:
+            requests.ConnectionError: Connection error
+            requests.ConnectionTimeout: Timed out connecting to AIStore
+            requests.exceptions.HTTPError: Service unavailable
+            requests.RequestException: "There was an ambiguous exception that occurred while handling..."
+            requests.ReadTimeout: Timed out receiving response from AIStore
+            aistore.sdk.errors.AISError: All other types of errors with AIStore
+        """
+        bsumm_ctrl_msg = BsummCtrlMsg(
+            uuid=uuid, prefix=prefix, fast=fast, cached=cached, present=present
+        )
+
+        # Start the job and get the job ID
+        resp = self.make_request(
+            HTTP_METHOD_GET,
+            ACT_SUMMARY_BCK,
+            params=self.qparam,
+            value=bsumm_ctrl_msg.dict(),
+        )
+
+        # Initial response status code should be 202
+        if resp.status_code == STATUS_OK:
+            raise UnexpectedHTTPStatusCode([STATUS_ACCEPTED], resp.status_code)
+
+        job_id = resp.text.strip('"')
+
+        # Update the uuid in the control message
+        bsumm_ctrl_msg.uuid = job_id
+
+        # Sleep and request frequency in sec (starts at 200 ms)
+        sleep_time = 0.2
+
+        # Poll async task for http.StatusOK completion
+        while True:
+            resp = self.make_request(
+                HTTP_METHOD_GET,
+                ACT_SUMMARY_BCK,
+                params=self.qparam,
+                value=bsumm_ctrl_msg.dict(),
+            )
+
+            # If task completed successfully, break the loop
+            if resp.status_code == STATUS_OK:
+                break
+            # If task is still running, wait for some time and try again
+            if resp.status_code == STATUS_ACCEPTED:
+                time.sleep(sleep_time)
+                sleep_time = min(
+                    10, sleep_time * 1.5
+                )  # Increase sleep_time by 50%, but don't exceed 10 seconds
+            # Otherwise, if status code received is neither STATUS_OK or STATUS_ACCEPTED, raise an exception
+            else:
+                raise UnexpectedHTTPStatusCode(
+                    [STATUS_OK, STATUS_ACCEPTED], resp.status_code
+                )
+
+        return json.loads(resp.content.decode("utf-8"))[0]
+
+    def info(self, flt_presence: int = 0, count_remote_objs: bool = True):
+        """
+        Returns bucket summary and information/properties.
+
+        Args:
+            count_remote_objs (bool): If True, returned bucket info will entail remote objects as well
+            flt_presence (int): Describes the presence of buckets and objects with respect to their existence
+                                or non-existence in the AIS cluster. Defaults to 0.
+
+                                Expected values are:
+                                0 - (object | bucket) exists inside and/or outside cluster
+                                1 - same as 0 but no need to return summary
+                                2 - bucket: is present | object: present and properly located
+                                3 - same as 2 but no need to return summary
+                                4 - objects: present anywhere/anyhow _in_ the cluster as: replica, ec-slices, misplaced
+                                5 - not present - exists _outside_ cluster
+
+        Raises:
+            requests.ConnectionError: Connection error
+            requests.ConnectionTimeout: Timed out connecting to AIStore
+            requests.exceptions.HTTPError: Service unavailable
+            requests.RequestException: "There was an ambiguous exception that occurred while handling..."
+            requests.ReadTimeout: Timed out receiving response from AIStore
+            ValueError: `flt_presence` is not one of the expected values
+            aistore.sdk.errors.AISError: All other types of errors with AIStore
+        """
+        if flt_presence not in range(6):
+            raise ValueError("`flt_presence` must be one of 0, 1, 2, 3, 4, or 5.")
+
+        params = self.qparam.copy()
+        params.update({QPARAM_FLT_PRESENCE: flt_presence})
+        if count_remote_objs:
+            params.update({QPARAM_COUNT_REMOTE_OBJS: count_remote_objs})
+
+        response = self.client.request(
+            HTTP_METHOD_HEAD,
+            path=f"{URL_PATH_BUCKETS}/{self.name}",
+            params=params,
+        )
+
+        bucket_props = json.loads(response.headers.get(HEADER_BUCKET_PROPS, "{}"))
+        bucket_summ = json.loads(response.headers.get(HEADER_BUCKET_SUMM, "{}"))
+
+        return bucket_props, bucket_summ
+
+    # pylint: disable=too-many-arguments
     def copy(
         self,
         to_bck: Bucket,
         prefix_filter: str = "",
         prepend: str = "",
         dry_run: bool = False,
         force: bool = False,
```

### Comparing `aistore-1.3.0/aistore/sdk/client.py` & `aistore-1.4.0/aistore/sdk/client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/cluster.py` & `aistore-1.4.0/aistore/sdk/cluster.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/const.py` & `aistore-1.4.0/aistore/sdk/const.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,27 @@
 MSGPACK_CONTENT_TYPE = "application/msgpack"
 # AIS Headers
 AIS_CHECKSUM_TYPE = "ais-checksum-type"
 AIS_CHECKSUM_VALUE = "ais-checksum-value"
 AIS_ACCESS_TIME = "ais-atime"
 AIS_VERSION = "ais-version"
 AIS_CUSTOM_MD = "ais-custom-md"
-
+# Bucket Props Header keys
+HEADER_PREFIX = "ais-"
+HEADER_BUCKET_PROPS = HEADER_PREFIX + "bucket-props"
+HEADER_BUCKET_SUMM = HEADER_PREFIX + "bucket-summ"
 
 # URL Params
 # See api/apc/query.go
 QPARAM_WHAT = "what"
 QPARAM_ETL_NAME = "etl_name"
 QPARAM_PROVIDER = "provider"
 QPARAM_BCK_TO = "bck_to"
+QPARAM_FLT_PRESENCE = "presence"
+QPARAM_COUNT_REMOTE_OBJS = "count_remote_objs"
 QPARAM_KEEP_REMOTE = "keep_bck_md"
 QPARAM_ARCHPATH = "archpath"
 QPARAM_FORCE = "frc"
 QPARAM_PRIMARY_READY_REB = "prr"
 QPARAM_NAMESPACE = "namespace"
 DSORT_UUID = "uuid"
 
@@ -73,14 +78,15 @@
 ACT_DESTROY_BCK = "destroy-bck"
 ACT_COPY_BCK = "copy-bck"
 ACT_ETL_BCK = "etl-bck"
 ACT_EVICT_REMOTE_BCK = "evict-remote-bck"
 ACT_LIST = "list"
 ACT_MOVE_BCK = "move-bck"
 ACT_PROMOTE = "promote"
+ACT_SUMMARY_BCK = "summary-bck"
 # Multi-object actions
 ACT_DELETE_OBJECTS = "delete-listrange"
 ACT_EVICT_OBJECTS = "evict-listrange"
 ACT_PREFETCH_OBJECTS = "prefetch-listrange"
 ACT_COPY_OBJECTS = "copy-listrange"
 ACT_TRANSFORM_OBJECTS = "etl-listrange"
 ACT_ARCHIVE_OBJECTS = "archive"
@@ -90,7 +96,12 @@
 # Defaults
 DEFAULT_CHUNK_SIZE = 32768
 DEFAULT_JOB_WAIT_TIMEOUT = 300
 DEFAULT_DSORT_WAIT_TIMEOUT = 300
 
 # ENCODING
 UTF_ENCODING = "utf-8"
+
+# Status Codes
+STATUS_ACCEPTED = 202
+STATUS_OK = 200
+STATUS_BAD_REQUEST = 400
```

### Comparing `aistore-1.3.0/aistore/sdk/dsort.py` & `aistore-1.4.0/aistore/sdk/dsort.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/dsort_types.py` & `aistore-1.4.0/aistore/sdk/dsort_types.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/errors.py` & `aistore-1.4.0/aistore/sdk/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,7 +87,23 @@
 class JobInfoNotFound(Exception):
     """
     Raised when information on a job's status could not be found on the AIS cluster
     """
 
     def __init__(self, message):
         super().__init__(f"Job information not found on the cluster: {message}")
+
+
+class UnexpectedHTTPStatusCode(Exception):
+    """
+    Raised when the status code from a response is not what's expected.
+    """
+
+    def __init__(self, expected_status_codes, received_status_code):
+        expected_codes = ", ".join(str(code) for code in expected_status_codes)
+        super().__init__(
+            (
+                f"Unexpected status code received. "
+                f"Expected one of the following: {expected_codes}, "
+                f"but received: {received_status_code}"
+            )
+        )
```

### Comparing `aistore-1.3.0/aistore/sdk/etl.py` & `aistore-1.4.0/aistore/sdk/etl.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/etl_const.py` & `aistore-1.4.0/aistore/sdk/etl_const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/etl_templates.py` & `aistore-1.4.0/aistore/sdk/etl_templates.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/job.py` & `aistore-1.4.0/aistore/sdk/job.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/list_object_flag.py` & `aistore-1.4.0/aistore/sdk/list_object_flag.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/object.py` & `aistore-1.4.0/aistore/sdk/object.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/object_attributes.py` & `aistore-1.4.0/aistore/sdk/object_attributes.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/object_iterator.py` & `aistore-1.4.0/aistore/sdk/object_iterator.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/object_reader.py` & `aistore-1.4.0/aistore/sdk/object_reader.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/request_client.py` & `aistore-1.4.0/aistore/sdk/request_client.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/types.py` & `aistore-1.4.0/aistore/sdk/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,26 @@
     def as_dict(self):
         dict_rep = {"name": self.name, "provider": self.provider}
         if self.namespace:
             dict_rep["namespace"] = self.namespace
         return dict_rep
 
 
+class BsummCtrlMsg(BaseModel):
+    """
+    Represents the bucket summary control message
+    """
+
+    uuid: str
+    prefix: str
+    fast: bool
+    cached: bool
+    present: bool
+
+
 class JobArgs(BaseModel):
     """
     Represents the set of args to pass when making a job-related request
     """
 
     id: str = ""
     kind: str = ""
```

### Comparing `aistore-1.3.0/aistore/sdk/utils.py` & `aistore-1.4.0/aistore/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/multiobj/object_collection.py` & `aistore-1.4.0/aistore/sdk/multiobj/object_collection.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/multiobj/object_group.py` & `aistore-1.4.0/aistore/sdk/multiobj/object_group.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/multiobj/object_names.py` & `aistore-1.4.0/aistore/sdk/multiobj/object_names.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/multiobj/object_range.py` & `aistore-1.4.0/aistore/sdk/multiobj/object_range.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/aistore/sdk/multiobj/object_template.py` & `aistore-1.4.0/aistore/sdk/multiobj/object_template.py`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/LICENSE` & `aistore-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/.gitignore` & `aistore-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/README.md` & `aistore-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/pyproject.toml` & `aistore-1.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aistore-1.3.0/PKG-INFO` & `aistore-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistore
-Version: 1.3.0
+Version: 1.4.0
 Summary: A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore.
 Project-URL: Homepage, https://aiatscale.org
 Project-URL: Download, https://github.com/NVIDIA/aistore/tags
 Project-URL: Documentation, https://aiatscale.org/docs/
 Project-URL: Release notes, https://github.com/NVIDIA/aistore/releases/
 Project-URL: Source, https://github.com/NVIDIA/aistore/
 Author-email: AIStore Team <ais@exchange.nvidia.com>
```

