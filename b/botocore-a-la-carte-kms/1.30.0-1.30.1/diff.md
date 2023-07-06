# Comparing `tmp/botocore-a-la-carte-kms-1.30.0.tar.gz` & `tmp/botocore-a-la-carte-kms-1.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-kms-1.30.0.tar", last modified: Tue Jul  4 01:44:42 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-kms-1.30.1.tar", last modified: Thu Jul  6 01:45:13 2023, max compression
```

## Comparing `botocore-a-la-carte-kms-1.30.0.tar` & `botocore-a-la-carte-kms-1.30.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-04 01:44:41.000000 botocore-a-la-carte-kms-1.30.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/botocore/data/kms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/
--rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-04 01:44:02.000000 botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    77655 2023-07-04 01:44:02.000000 botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-04 01:44:02.000000 botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   432454 2023-07-04 01:44:02.000000 botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/botocore_a_la_carte_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-04 01:44:42.000000 botocore-a-la-carte-kms-1.30.0/botocore_a_la_carte_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-04 01:44:42.000000 botocore-a-la-carte-kms-1.30.0/botocore_a_la_carte_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 01:44:42.000000 botocore-a-la-carte-kms-1.30.0/botocore_a_la_carte_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 01:44:42.000000 botocore-a-la-carte-kms-1.30.0/botocore_a_la_carte_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 01:44:42.194665 botocore-a-la-carte-kms-1.30.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-04 01:44:41.000000 botocore-a-la-carte-kms-1.30.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:13.194930 botocore-a-la-carte-kms-1.30.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-06 01:45:12.000000 botocore-a-la-carte-kms-1.30.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 01:45:13.194930 botocore-a-la-carte-kms-1.30.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:13.190930 botocore-a-la-carte-kms-1.30.1/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:13.190930 botocore-a-la-carte-kms-1.30.1/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:13.190930 botocore-a-la-carte-kms-1.30.1/botocore/data/kms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:13.190930 botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    17612 2023-07-06 01:44:40.000000 botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    77655 2023-07-06 01:44:40.000000 botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-06 01:44:40.000000 botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   439338 2023-07-06 01:44:40.000000 botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 01:45:13.190930 botocore-a-la-carte-kms-1.30.1/botocore_a_la_carte_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 01:45:13.000000 botocore-a-la-carte-kms-1.30.1/botocore_a_la_carte_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-06 01:45:13.000000 botocore-a-la-carte-kms-1.30.1/botocore_a_la_carte_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 01:45:13.000000 botocore-a-la-carte-kms-1.30.1/botocore_a_la_carte_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 01:45:13.000000 botocore-a-la-carte-kms-1.30.1/botocore_a_la_carte_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 01:45:13.194930 botocore-a-la-carte-kms-1.30.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-06 01:45:12.000000 botocore-a-la-carte-kms-1.30.1/setup.py
```

### Comparing `botocore-a-la-carte-kms-1.30.0/LICENSE.txt` & `botocore-a-la-carte-kms-1.30.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kms-1.30.0/PKG-INFO` & `botocore-a-la-carte-kms-1.30.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-kms
-Version: 1.30.0
+Version: 1.30.1
 Summary: kms data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/examples-1.json` & `botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/paginators-1.json` & `botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-kms-1.30.0/botocore/data/kms/2014-11-01/service-2.json` & `botocore-a-la-carte-kms-1.30.1/botocore/data/kms/2014-11-01/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992255818266378%*

 * *Differences: {"'operations'": "{'CreateGrant': {'errors': {insert: [(8, OrderedDict([('shape', "*

 * *                 "'DryRunOperationException')]))]}}, 'Decrypt': {'errors': {insert: [(10, "*

 * *                 "OrderedDict([('shape', 'DryRunOperationException')]))]}}, 'Encrypt': {'errors': "*

 * *                 "{insert: [(8, OrderedDict([('shape', 'DryRunOperationException')]))]}}, "*

 * *                 "'GenerateDataKey': {'errors': {insert: [(8, OrderedDict([('shape', "*

 * *                 "'DryRunOperationException')]))]}}, 'Gen […]*

```diff
@@ -198,14 +198,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "LimitExceededException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -299,14 +302,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -628,14 +634,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -668,14 +677,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -711,14 +723,17 @@
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
                 },
                 {
                     "shape": "UnsupportedOperationException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -754,14 +769,17 @@
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
                 },
                 {
                     "shape": "UnsupportedOperationException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -794,14 +812,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -831,14 +852,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1319,14 +1343,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1402,14 +1429,17 @@
                     "shape": "DependencyTimeoutException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1433,27 +1463,30 @@
                     "shape": "InvalidGrantIdException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RevokeGrantRequest"
             },
             "name": "RevokeGrant"
         },
         "ScheduleKeyDeletion": {
-            "documentation": "<p>Schedules the deletion of a KMS key. By default, KMS applies a waiting period of 30 days, but you can specify a waiting period of 7-30 days. When this operation is successful, the key state of the KMS key changes to <code>PendingDeletion</code> and the key can't be used in any cryptographic operations. It remains in this state for the duration of the waiting period. Before the waiting period ends, you can use <a>CancelKeyDeletion</a> to cancel the deletion of the KMS key. After the waiting period ends, KMS deletes the KMS key, its key material, and all KMS data associated with it, including all aliases that refer to it.</p> <important> <p>Deleting a KMS key is a destructive and potentially dangerous operation. When a KMS key is deleted, all data that was encrypted under the KMS key is unrecoverable. (The only exception is a <a href=\"kms/latest/developerguide/multi-region-keys-delete.html\">multi-Region replica key</a>, or an asymmetric or HMAC KMS key with imported key material[BUGBUG-link to importing-keys-managing.html#import-delete-key.) To prevent the use of a KMS key without deleting it, use <a>DisableKey</a>. </p> </important> <p>You can schedule the deletion of a multi-Region primary key and its replica keys at any time. However, KMS will not delete a multi-Region primary key with existing replica keys. If you schedule the deletion of a primary key with replicas, its key state changes to <code>PendingReplicaDeletion</code> and it cannot be replicated or used in cryptographic operations. This status can continue indefinitely. When the last of its replicas keys is deleted (not just scheduled), the key state of the primary key changes to <code>PendingDeletion</code> and its waiting period (<code>PendingWindowInDays</code>) begins. For details, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/multi-region-keys-delete.html\">Deleting multi-Region keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p>When KMS <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/delete-cmk-keystore.html\">deletes a KMS key from an CloudHSM key store</a>, it makes a best effort to delete the associated key material from the associated CloudHSM cluster. However, you might need to manually <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/fix-keystore.html#fix-keystore-orphaned-key\">delete the orphaned key material</a> from the cluster and its backups. <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/delete-xks-key.html\">Deleting a KMS key from an external key store</a> has no effect on the associated external key. However, for both types of custom key stores, deleting a KMS key is destructive and irreversible. You cannot decrypt ciphertext encrypted under the KMS key by using only its associated external key or CloudHSM key. Also, you cannot recreate a KMS key in an external key store by creating a new KMS key with the same key material.</p> <p>For more information about scheduling a KMS key for deletion, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/deleting-keys.html\">Deleting KMS keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p>The KMS key that you use for this operation must be in a compatible key state. For details, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html\">Key states of KMS keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p> <b>Cross-account use</b>: No. You cannot perform this operation on a KMS key in a different Amazon Web Services account.</p> <p> <b>Required permissions</b>: kms:ScheduleKeyDeletion (key policy)</p> <p> <b>Related operations</b> </p> <ul> <li> <p> <a>CancelKeyDeletion</a> </p> </li> <li> <p> <a>DisableKey</a> </p> </li> </ul>",
+            "documentation": "<p>Schedules the deletion of a KMS key. By default, KMS applies a waiting period of 30 days, but you can specify a waiting period of 7-30 days. When this operation is successful, the key state of the KMS key changes to <code>PendingDeletion</code> and the key can't be used in any cryptographic operations. It remains in this state for the duration of the waiting period. Before the waiting period ends, you can use <a>CancelKeyDeletion</a> to cancel the deletion of the KMS key. After the waiting period ends, KMS deletes the KMS key, its key material, and all KMS data associated with it, including all aliases that refer to it.</p> <important> <p>Deleting a KMS key is a destructive and potentially dangerous operation. When a KMS key is deleted, all data that was encrypted under the KMS key is unrecoverable. (The only exception is a <a href=\"kms/latest/developerguide/multi-region-keys-delete.html\">multi-Region replica key</a>, or an <a href=\"kms/latest/developerguide/importing-keys-managing.html#import-delete-key\">asymmetric or HMAC KMS key with imported key material</a>.) To prevent the use of a KMS key without deleting it, use <a>DisableKey</a>. </p> </important> <p>You can schedule the deletion of a multi-Region primary key and its replica keys at any time. However, KMS will not delete a multi-Region primary key with existing replica keys. If you schedule the deletion of a primary key with replicas, its key state changes to <code>PendingReplicaDeletion</code> and it cannot be replicated or used in cryptographic operations. This status can continue indefinitely. When the last of its replicas keys is deleted (not just scheduled), the key state of the primary key changes to <code>PendingDeletion</code> and its waiting period (<code>PendingWindowInDays</code>) begins. For details, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/multi-region-keys-delete.html\">Deleting multi-Region keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p>When KMS <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/delete-cmk-keystore.html\">deletes a KMS key from an CloudHSM key store</a>, it makes a best effort to delete the associated key material from the associated CloudHSM cluster. However, you might need to manually <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/fix-keystore.html#fix-keystore-orphaned-key\">delete the orphaned key material</a> from the cluster and its backups. <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/delete-xks-key.html\">Deleting a KMS key from an external key store</a> has no effect on the associated external key. However, for both types of custom key stores, deleting a KMS key is destructive and irreversible. You cannot decrypt ciphertext encrypted under the KMS key by using only its associated external key or CloudHSM key. Also, you cannot recreate a KMS key in an external key store by creating a new KMS key with the same key material.</p> <p>For more information about scheduling a KMS key for deletion, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/deleting-keys.html\">Deleting KMS keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p>The KMS key that you use for this operation must be in a compatible key state. For details, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/key-state.html\">Key states of KMS keys</a> in the <i>Key Management Service Developer Guide</i>.</p> <p> <b>Cross-account use</b>: No. You cannot perform this operation on a KMS key in a different Amazon Web Services account.</p> <p> <b>Required permissions</b>: kms:ScheduleKeyDeletion (key policy)</p> <p> <b>Related operations</b> </p> <ul> <li> <p> <a>CancelKeyDeletion</a> </p> </li> <li> <p> <a>DisableKey</a> </p> </li> </ul>",
             "errors": [
                 {
                     "shape": "NotFoundException"
                 },
                 {
                     "shape": "InvalidArnException"
                 },
@@ -1501,14 +1534,17 @@
                     "shape": "InvalidGrantTokenException"
                 },
                 {
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1757,14 +1793,17 @@
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
                 },
                 {
                     "shape": "KMSInvalidSignatureException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -1797,14 +1836,17 @@
                     "shape": "KMSInternalException"
                 },
                 {
                     "shape": "KMSInvalidMacException"
                 },
                 {
                     "shape": "KMSInvalidStateException"
+                },
+                {
+                    "shape": "DryRunOperationException"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -2098,14 +2140,18 @@
         },
         "CreateGrantRequest": {
             "members": {
                 "Constraints": {
                     "documentation": "<p>Specifies a grant constraint.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>KMS supports the <code>EncryptionContextEquals</code> and <code>EncryptionContextSubset</code> grant constraints, which allow the permissions in the grant only when the encryption context in the request matches (<code>EncryptionContextEquals</code>) or includes (<code>EncryptionContextSubset</code>) the encryption context specified in the constraint. </p> <p>The encryption context grant constraints are supported only on <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#terms-grant-operations\">grant operations</a> that include an <code>EncryptionContext</code> parameter, such as cryptographic operations on symmetric encryption KMS keys. Grants with grant constraints can include the <a>DescribeKey</a> and <a>RetireGrant</a> operations, but the constraint doesn't apply to these operations. If a grant with a grant constraint includes the <code>CreateGrant</code> operation, the constraint requires that any grants created with the <code>CreateGrant</code> permission have an equally strict or stricter encryption context constraint.</p> <p>You cannot use an encryption context grant constraint for cryptographic operations with asymmetric KMS keys or HMAC KMS keys. Operations with these keys don't support an encryption context.</p> <p>Each constraint value can include up to 8 encryption context pairs. The encryption context value in each constraint cannot exceed 384 characters. For information about grant constraints, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/create-grant-overview.html#grant-constraints\">Using grant constraints</a> in the <i>Key Management Service Developer Guide</i>. For more information about encryption context, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i> <i>Key Management Service Developer Guide</i> </i>. </p>",
                     "shape": "GrantConstraints"
                 },
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens. </p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
                 },
                 "GranteePrincipal": {
                     "documentation": "<p>The identity that gets the permissions specified in the grant.</p> <p>To specify the grantee principal, use the Amazon Resource Name (ARN) of an Amazon Web Services principal. Valid principals include Amazon Web Services accounts, IAM users, IAM roles, federated users, and assumed role users. For help with the ARN syntax for a principal, see <a href=\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html#identifiers-arns\">IAM ARNs</a> in the <i> <i>Identity and Access Management User Guide</i> </i>.</p>",
                     "shape": "PrincipalIdType"
@@ -2357,14 +2403,18 @@
         },
         "DecryptRequest": {
             "members": {
                 "CiphertextBlob": {
                     "documentation": "<p>Ciphertext to be decrypted. The blob includes metadata.</p>",
                     "shape": "CiphertextType"
                 },
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "EncryptionAlgorithm": {
                     "documentation": "<p>Specifies the encryption algorithm that will be used to decrypt the ciphertext. Specify the same algorithm that was used to encrypt the data. If you specify a different algorithm, the <code>Decrypt</code> operation fails.</p> <p>This parameter is required only when the ciphertext was encrypted under an asymmetric KMS key. The default value, <code>SYMMETRIC_DEFAULT</code>, represents the only supported algorithm that is valid for symmetric encryption KMS keys.</p>",
                     "shape": "EncryptionAlgorithmSpec"
                 },
                 "EncryptionContext": {
                     "documentation": "<p>Specifies the encryption context to use when decrypting the data. An encryption context is valid only for <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations\">cryptographic operations</a> with a symmetric encryption KMS key. The standard asymmetric encryption algorithms and HMAC algorithms that KMS uses do not support an encryption context.</p> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
@@ -2573,14 +2623,24 @@
             ],
             "type": "structure"
         },
         "DisconnectCustomKeyStoreResponse": {
             "members": {},
             "type": "structure"
         },
+        "DryRunOperationException": {
+            "documentation": "<p> The request was rejected because the DryRun parameter was specified. </p>",
+            "exception": true,
+            "members": {
+                "message": {
+                    "shape": "ErrorMessageType"
+                }
+            },
+            "type": "structure"
+        },
         "EnableKeyRequest": {
             "members": {
                 "KeyId": {
                     "documentation": "<p>Identifies the KMS key to enable.</p> <p>Specify the key ID or key ARN of the KMS key.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> </ul> <p>To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>.</p>",
                     "shape": "KeyIdType"
                 }
             },
@@ -2599,14 +2659,18 @@
             "required": [
                 "KeyId"
             ],
             "type": "structure"
         },
         "EncryptRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "EncryptionAlgorithm": {
                     "documentation": "<p>Specifies the encryption algorithm that KMS will use to encrypt the plaintext message. The algorithm must be compatible with the KMS key that you specify.</p> <p>This parameter is required only for asymmetric KMS keys. The default value, <code>SYMMETRIC_DEFAULT</code>, is the algorithm used for symmetric encryption KMS keys. If you are using an asymmetric KMS key, we recommend RSAES_OAEP_SHA_256.</p> <p>The SM2PKE algorithm is only available in China Regions.</p>",
                     "shape": "EncryptionAlgorithmSpec"
                 },
                 "EncryptionContext": {
                     "documentation": "<p>Specifies the encryption context that will be used to encrypt the data. An encryption context is valid only for <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#cryptographic-operations\">cryptographic operations</a> with a symmetric encryption KMS key. The standard asymmetric encryption algorithms and HMAC algorithms that KMS uses do not support an encryption context. </p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
@@ -2695,14 +2759,18 @@
                     "shape": "ErrorMessageType"
                 }
             },
             "type": "structure"
         },
         "GenerateDataKeyPairRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "EncryptionContext": {
                     "documentation": "<p>Specifies the encryption context that will be used when encrypting the private key in the data key pair.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
                 },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
@@ -2753,14 +2821,18 @@
                     "shape": "PublicKeyType"
                 }
             },
             "type": "structure"
         },
         "GenerateDataKeyPairWithoutPlaintextRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "EncryptionContext": {
                     "documentation": "<p>Specifies the encryption context that will be used when encrypting the private key in the data key pair.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
                 },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
@@ -2799,14 +2871,18 @@
                     "shape": "PublicKeyType"
                 }
             },
             "type": "structure"
         },
         "GenerateDataKeyRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "EncryptionContext": {
                     "documentation": "<p>Specifies the encryption context that will be used when encrypting the data key.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
                 },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
@@ -2852,14 +2928,18 @@
                     "shape": "PlaintextType"
                 }
             },
             "type": "structure"
         },
         "GenerateDataKeyWithoutPlaintextRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "EncryptionContext": {
                     "documentation": "<p>Specifies the encryption context that will be used when encrypting the data key.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
                 },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
@@ -2893,14 +2973,18 @@
                     "shape": "KeyIdType"
                 }
             },
             "type": "structure"
         },
         "GenerateMacRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
                 },
                 "KeyId": {
                     "documentation": "<p>The HMAC KMS key to use in the operation. The MAC algorithm computes the HMAC for the message and the key as described in <a href=\"https://datatracker.ietf.org/doc/html/rfc2104\">RFC 2104</a>.</p> <p>To identify an HMAC KMS key, use the <a>DescribeKey</a> operation and see the <code>KeySpec</code> field in the response.</p>",
                     "shape": "KeyIdType"
@@ -4016,14 +4100,18 @@
                     "documentation": "<p>Specifies that encryption context to use when the reencrypting the data.</p> <important> <p>Do not include confidential or sensitive information in this field. This field may be displayed in plaintext in CloudTrail logs and other output.</p> </important> <p>A destination encryption context is valid only when the destination KMS key is a symmetric encryption KMS key. The standard ciphertext format for asymmetric KMS keys does not include fields for metadata.</p> <p>An <i>encryption context</i> is a collection of non-secret key-value pairs that represent additional authenticated data. When you use an encryption context to encrypt data, you must specify the same (an exact case-sensitive match) encryption context to decrypt the data. An encryption context is supported only on operations with symmetric encryption KMS keys. On operations with symmetric encryption KMS keys, an encryption context is optional, but it is strongly recommended.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#encrypt_context\">Encryption context</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "EncryptionContextType"
                 },
                 "DestinationKeyId": {
                     "documentation": "<p>A unique identifier for the KMS key that is used to reencrypt the data. Specify a symmetric encryption KMS key or an asymmetric KMS key with a <code>KeyUsage</code> value of <code>ENCRYPT_DECRYPT</code>. To find the <code>KeyUsage</code> value of a KMS key, use the <a>DescribeKey</a> operation.</p> <p>To specify a KMS key, use its key ID, key ARN, alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a KMS key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>. To get the alias name and alias ARN, use <a>ListAliases</a>.</p>",
                     "shape": "KeyIdType"
                 },
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
                 },
                 "SourceEncryptionAlgorithm": {
                     "documentation": "<p>Specifies the encryption algorithm that KMS will use to decrypt the ciphertext before it is reencrypted. The default value, <code>SYMMETRIC_DEFAULT</code>, represents the algorithm used for symmetric encryption KMS keys.</p> <p>Specify the same algorithm that was used to encrypt the ciphertext. If you specify a different algorithm, the decrypt attempt fails.</p> <p>This parameter is required only when the ciphertext was encrypted under an asymmetric KMS key.</p>",
                     "shape": "EncryptionAlgorithmSpec"
@@ -4136,14 +4224,18 @@
                     "shape": "TagList"
                 }
             },
             "type": "structure"
         },
         "RetireGrantRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantId": {
                     "documentation": "<p>Identifies the grant to retire. To get the grant ID, use <a>CreateGrant</a>, <a>ListGrants</a>, or <a>ListRetirableGrants</a>.</p> <ul> <li> <p>Grant ID Example - 0123456789012345678901234567890123456789012345678901234567890123</p> </li> </ul>",
                     "shape": "GrantIdType"
                 },
                 "GrantToken": {
                     "documentation": "<p>Identifies the grant to be retired. You can use a grant token to identify a new grant even before it has achieved eventual consistency.</p> <p>Only the <a>CreateGrant</a> operation returns a grant token. For details, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#terms-eventual-consistency\">Eventual consistency</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenType"
@@ -4153,14 +4245,18 @@
                     "shape": "KeyIdType"
                 }
             },
             "type": "structure"
         },
         "RevokeGrantRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantId": {
                     "documentation": "<p>Identifies the grant to revoke. To get the grant ID, use <a>CreateGrant</a>, <a>ListGrants</a>, or <a>ListRetirableGrants</a>.</p>",
                     "shape": "GrantIdType"
                 },
                 "KeyId": {
                     "documentation": "<p>A unique identifier for the KMS key associated with the grant. To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>.</p> <p>Specify the key ID or key ARN of the KMS key. To specify a KMS key in a different Amazon Web Services account, you must use the key ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> </ul> <p>To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>.</p>",
                     "shape": "KeyIdType"
@@ -4175,15 +4271,15 @@
         "ScheduleKeyDeletionRequest": {
             "members": {
                 "KeyId": {
                     "documentation": "<p>The unique identifier of the KMS key to delete.</p> <p>Specify the key ID or key ARN of the KMS key.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> </ul> <p>To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>.</p>",
                     "shape": "KeyIdType"
                 },
                 "PendingWindowInDays": {
-                    "documentation": "<p>The waiting period, specified in number of days. After the waiting period ends, KMS deletes the KMS key.</p> <p>If the KMS key is a multi-Region primary key with replica keys, the waiting period begins when the last of its replica keys is deleted. Otherwise, the waiting period begins immediately.</p> <p>This value is optional. If you include a value, it must be between 7 and 30, inclusive. If you do not include a value, it defaults to 30. You can use the <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/conditions-kms.html#conditions-pending-deletion-window\"> <code>kms:ScheduleKeyDeletionPendingWindowInDays</code> </a> condition key to further constrain the values that principals can specify in the <code>PendingWindowInDays</code> parameter.</p>",
+                    "documentation": "<p>The waiting period, specified in number of days. After the waiting period ends, KMS deletes the KMS key.</p> <p>If the KMS key is a multi-Region primary key with replica keys, the waiting period begins when the last of its replica keys is deleted. Otherwise, the waiting period begins immediately.</p> <p>This value is optional. If you include a value, it must be between 7 and 30, inclusive. If you do not include a value, it defaults to 30. You can use the <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/conditions-kms.html#conditions-kms-schedule-key-deletion-pending-window-in-days\"> <code>kms:ScheduleKeyDeletionPendingWindowInDays</code> </a> condition key to further constrain the values that principals can specify in the <code>PendingWindowInDays</code> parameter.</p>",
                     "shape": "PendingWindowInDaysType"
                 }
             },
             "required": [
                 "KeyId"
             ],
             "type": "structure"
@@ -4207,14 +4303,18 @@
                     "shape": "PendingWindowInDaysType"
                 }
             },
             "type": "structure"
         },
         "SignRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
                 },
                 "KeyId": {
                     "documentation": "<p>Identifies an asymmetric KMS key. KMS uses the private key in the asymmetric KMS key to sign the message. The <code>KeyUsage</code> type of the KMS key must be <code>SIGN_VERIFY</code>. To find the <code>KeyUsage</code> of a KMS key, use the <a>DescribeKey</a> operation.</p> <p>To specify a KMS key, use its key ID, key ARN, alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a KMS key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>. To get the alias name and alias ARN, use <a>ListAliases</a>.</p>",
                     "shape": "KeyIdType"
@@ -4473,14 +4573,18 @@
                 "KeyId",
                 "PrimaryRegion"
             ],
             "type": "structure"
         },
         "VerifyMacRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
                 },
                 "KeyId": {
                     "documentation": "<p>The KMS key that will be used in the verification.</p> <p>Enter a key ID of the KMS key that was used to generate the HMAC. If you identify a different KMS key, the <code>VerifyMac</code> operation fails.</p>",
                     "shape": "KeyIdType"
@@ -4521,14 +4625,18 @@
                     "shape": "BooleanType"
                 }
             },
             "type": "structure"
         },
         "VerifyRequest": {
             "members": {
+                "DryRun": {
+                    "documentation": "<p>Checks if your request will succeed. <code>DryRun</code> is an optional parameter. </p> <p>To learn more about how to use this parameter, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/programming-dryrun.html\">Testing your KMS API calls</a> in the <i>Key Management Service Developer Guide</i>.</p>",
+                    "shape": "NullableBooleanType"
+                },
                 "GrantTokens": {
                     "documentation": "<p>A list of grant tokens.</p> <p>Use a grant token when your permission to call this operation comes from a new grant that has not yet achieved <i>eventual consistency</i>. For more information, see <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grants.html#grant_token\">Grant token</a> and <a href=\"https://docs.aws.amazon.com/kms/latest/developerguide/grant-manage.html#using-grant-token\">Using a grant token</a> in the <i>Key Management Service Developer Guide</i>.</p>",
                     "shape": "GrantTokenList"
                 },
                 "KeyId": {
                     "documentation": "<p>Identifies the asymmetric KMS key that will be used to verify the signature. This must be the same KMS key that was used to generate the signature. If you specify a different KMS key, the signature verification fails.</p> <p>To specify a KMS key, use its key ID, key ARN, alias name, or alias ARN. When using an alias name, prefix it with <code>\"alias/\"</code>. To specify a KMS key in a different Amazon Web Services account, you must use the key ARN or alias ARN.</p> <p>For example:</p> <ul> <li> <p>Key ID: <code>1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Key ARN: <code>arn:aws:kms:us-east-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab</code> </p> </li> <li> <p>Alias name: <code>alias/ExampleAlias</code> </p> </li> <li> <p>Alias ARN: <code>arn:aws:kms:us-east-2:111122223333:alias/ExampleAlias</code> </p> </li> </ul> <p>To get the key ID and key ARN for a KMS key, use <a>ListKeys</a> or <a>DescribeKey</a>. To get the alias name and alias ARN, use <a>ListAliases</a>.</p>",
                     "shape": "KeyIdType"
```

### Comparing `botocore-a-la-carte-kms-1.30.0/botocore_a_la_carte_kms.egg-info/PKG-INFO` & `botocore-a-la-carte-kms-1.30.1/botocore_a_la_carte_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-kms
-Version: 1.30.0
+Version: 1.30.1
 Summary: kms data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-kms-1.30.0/setup.py` & `botocore-a-la-carte-kms-1.30.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-kms',
-    version="1.30.0",
+    version="1.30.1",
     description='kms data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/kms/*/*.json'],
```

