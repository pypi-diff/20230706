# Comparing `tmp/falu-1.0.1.tar.gz` & `tmp/falu-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falu-1.0.1.tar", last modified: Wed Apr 19 06:45:20 2023, max compression
+gzip compressed data, was "falu-1.0.2.tar", last modified: Thu Jul  6 05:50:26 2023, max compression
```

## Comparing `falu-1.0.1.tar` & `falu-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:20.089457 falu-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 06:45:05.000000 falu-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-19 06:45:20.089457 falu-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-04-19 06:45:05.000000 falu-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:20.085457 falu-1.0.1/falu/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 06:45:05.000000 falu-1.0.1/falu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:20.085457 falu-1.0.1/falu/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:05.000000 falu-1.0.1/falu/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-19 06:45:05.000000 falu-1.0.1/falu/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-19 06:45:05.000000 falu-1.0.1/falu/client/falu_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-19 06:45:05.000000 falu-1.0.1/falu/client/json_patch_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-19 06:45:05.000000 falu-1.0.1/falu/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:20.089457 falu-1.0.1/falu/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:05.000000 falu-1.0.1/falu/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-19 06:45:05.000000 falu-1.0.1/falu/generic/delete_api_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-19 06:45:05.000000 falu-1.0.1/falu/generic/get_api_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-19 06:45:05.000000 falu-1.0.1/falu/generic/patch_api_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-19 06:45:05.000000 falu-1.0.1/falu/generic/post_api_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-19 06:45:05.000000 falu-1.0.1/falu/list_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-19 06:45:05.000000 falu-1.0.1/falu/query_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-19 06:45:05.000000 falu-1.0.1/falu/range_filtering_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:20.089457 falu-1.0.1/falu/services/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/file_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/identity_verification_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/identity_verifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/message_batches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/message_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/message_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/message_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/money.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/payment_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/payment_refunds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/temporary_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/terminal_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/terminal_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/terminal_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/transfer_reversals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/visitor_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/visits.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/wallet_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-19 06:45:05.000000 falu-1.0.1/falu/services/webhook_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-19 06:45:05.000000 falu-1.0.1/falu/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:45:20.085457 falu-1.0.1/falu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-19 06:45:20.000000 falu-1.0.1/falu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-19 06:45:20.000000 falu-1.0.1/falu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:45:20.000000 falu-1.0.1/falu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:45:20.000000 falu-1.0.1/falu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-19 06:45:20.000000 falu-1.0.1/falu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 06:45:20.000000 falu-1.0.1/falu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-19 06:45:05.000000 falu-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-19 06:45:20.089457 falu-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-19 06:45:05.000000 falu-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:26.692000 falu-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 05:50:12.000000 falu-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 05:50:26.692000 falu-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-06 05:50:12.000000 falu-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:26.688000 falu-1.0.2/falu/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-06 05:50:12.000000 falu-1.0.2/falu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:26.688000 falu-1.0.2/falu/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:12.000000 falu-1.0.2/falu/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-06 05:50:12.000000 falu-1.0.2/falu/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-06 05:50:12.000000 falu-1.0.2/falu/client/falu_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-06 05:50:12.000000 falu-1.0.2/falu/client/json_patch_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-06 05:50:12.000000 falu-1.0.2/falu/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:26.688000 falu-1.0.2/falu/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:12.000000 falu-1.0.2/falu/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 05:50:12.000000 falu-1.0.2/falu/generic/delete_api_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 05:50:12.000000 falu-1.0.2/falu/generic/get_api_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 05:50:12.000000 falu-1.0.2/falu/generic/patch_api_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 05:50:12.000000 falu-1.0.2/falu/generic/post_api_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-06 05:50:12.000000 falu-1.0.2/falu/list_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-06 05:50:12.000000 falu-1.0.2/falu/query_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-06 05:50:12.000000 falu-1.0.2/falu/range_filtering_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:26.692000 falu-1.0.2/falu/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/file_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/identity_verification_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/identity_verifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/message_batches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/message_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/message_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/message_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/money.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/payment_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/payment_refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/temporary_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/terminal_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/terminal_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/terminal_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/transfer_reversals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/visitor_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/visits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-06 05:50:12.000000 falu-1.0.2/falu/services/webhook_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 05:50:12.000000 falu-1.0.2/falu/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:50:26.688000 falu-1.0.2/falu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 05:50:26.000000 falu-1.0.2/falu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 05:50:26.000000 falu-1.0.2/falu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:50:26.000000 falu-1.0.2/falu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:50:26.000000 falu-1.0.2/falu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 05:50:26.000000 falu-1.0.2/falu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 05:50:26.000000 falu-1.0.2/falu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 05:50:12.000000 falu-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-06 05:50:26.692000 falu-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-06 05:50:12.000000 falu-1.0.2/setup.py
```

### Comparing `falu-1.0.1/LICENSE` & `falu-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/PKG-INFO` & `falu-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: falu
-Version: 1.0.1
+Version: 1.0.2
 Summary: The official Falu Python library
-Home-page: https://github.com/tinglesoftware/falu-python
+Home-page: https://github.com/faluapp/falu-python
 Author: Falu
-Author-email: info@tingle.software
+Author-email: support@falu.io
 License: MIT
 Keywords: falu api payments
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `falu-1.0.1/README.md` & `falu-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -73,10 +73,10 @@
 the [MIT](http://www.opensource.org/licenses/mit-license.php "Read more about the MIT license form") license. Refer to
 the [LICENSE](./LICENSE) file for more information.
 
 [dashboard]: https://dashboard.falu.io
 
 [api-docs]: https://docs.falu.io/api?lang=python
 
-[issues]: https://github.com/tingle/falu-python/issues/new
+[issues]: https://github.com/faluapp/falu-python/issues/new
 
-[pulls]: https://github.com/tingle/falu-python/pulls
+[pulls]: https://github.com/faluapp/falu-python/pulls
```

#### html2text {}

```diff
@@ -15,9 +15,9 @@
 falu.Messages.get_messages(message_id='msg_2mONJ2DZEVRy6jrfP8HUhemd8PJ',
 api_key="fskt_test_...", workspace="wksp_...", live=False) ``` ## Development
 For any requests, bug or comments, please [open an issue][issues] or [submit a
 pull request][pulls]. The Library is licensed under the [MIT](http://
 www.opensource.org/licenses/mit-license.php "Read more about the MIT license
 form") license. Refer to the [LICENSE](./LICENSE) file for more information.
 [dashboard]: https://dashboard.falu.io [api-docs]: https://docs.falu.io/
-api?lang=python [issues]: https://github.com/tingle/falu-python/issues/new
-[pulls]: https://github.com/tingle/falu-python/pulls
+api?lang=python [issues]: https://github.com/faluapp/falu-python/issues/new
+[pulls]: https://github.com/faluapp/falu-python/pulls
```

### Comparing `falu-1.0.1/falu/client/api_client.py` & `falu-1.0.2/falu/client/api_client.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/client/falu_model.py` & `falu-1.0.2/falu/client/falu_model.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/client/json_patch_document.py` & `falu-1.0.2/falu/client/json_patch_document.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/errors.py` & `falu-1.0.2/falu/errors.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/list_options.py` & `falu-1.0.2/falu/list_options.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/query_values.py` & `falu-1.0.2/falu/query_values.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/__init__.py` & `falu-1.0.2/falu/services/__init__.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/customers.py` & `falu-1.0.2/falu/services/customers.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/events.py` & `falu-1.0.2/falu/services/events.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/file_links.py` & `falu-1.0.2/falu/services/file_links.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/files.py` & `falu-1.0.2/falu/services/files.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/identity_verification_reports.py` & `falu-1.0.2/falu/services/identity_verification_reports.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/identity_verifications.py` & `falu-1.0.2/falu/services/identity_verifications.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/message_batches.py` & `falu-1.0.2/falu/services/message_batches.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/message_streams.py` & `falu-1.0.2/falu/services/message_streams.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/message_suppressions.py` & `falu-1.0.2/falu/services/message_suppressions.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/message_templates.py` & `falu-1.0.2/falu/services/message_templates.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/messages.py` & `falu-1.0.2/falu/services/messages.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/money.py` & `falu-1.0.2/falu/services/money.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/payment_authorizations.py` & `falu-1.0.2/falu/services/payment_authorizations.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/payment_refunds.py` & `falu-1.0.2/falu/services/payment_refunds.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/payments.py` & `falu-1.0.2/falu/services/payments.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/temporary_keys.py` & `falu-1.0.2/falu/services/temporary_keys.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/terminal_configurations.py` & `falu-1.0.2/falu/services/terminal_configurations.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/terminal_devices.py` & `falu-1.0.2/falu/services/terminal_devices.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/terminal_locations.py` & `falu-1.0.2/falu/services/terminal_locations.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/transfer_reversals.py` & `falu-1.0.2/falu/services/transfer_reversals.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/transfers.py` & `falu-1.0.2/falu/services/transfers.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/visitor_destinations.py` & `falu-1.0.2/falu/services/visitor_destinations.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/visitors.py` & `falu-1.0.2/falu/services/visitors.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/visits.py` & `falu-1.0.2/falu/services/visits.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/wallet.py` & `falu-1.0.2/falu/services/wallet.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/wallet_transactions.py` & `falu-1.0.2/falu/services/wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu/services/webhook_endpoints.py` & `falu-1.0.2/falu/services/webhook_endpoints.py`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/falu.egg-info/PKG-INFO` & `falu-1.0.2/falu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: falu
-Version: 1.0.1
+Version: 1.0.2
 Summary: The official Falu Python library
-Home-page: https://github.com/tinglesoftware/falu-python
+Home-page: https://github.com/faluapp/falu-python
 Author: Falu
-Author-email: info@tingle.software
+Author-email: support@falu.io
 License: MIT
 Keywords: falu api payments
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `falu-1.0.1/falu.egg-info/SOURCES.txt` & `falu-1.0.2/falu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falu-1.0.1/setup.py` & `falu-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 setup(
     name='falu',
     version=version["VERSION"],
     description='The official Falu Python library',
     long_description=open("long_description.rst").read(),
     long_description_content_type="text/x-rst",
-    url='https://github.com/tinglesoftware/falu-python',
+    url='https://github.com/faluapp/falu-python',
     author='Falu',
-    author_email='info@tingle.software',
+    author_email='support@falu.io',
     keywords=["falu api payments"],
     zip_safe=False,
     license='MIT',
     python_requires=">=3.7",
     packages=find_packages(exclude=["tests", "tests.*"]),
     install_requires=[
         "pytest>=7.0.0",
```

