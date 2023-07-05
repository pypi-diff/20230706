# Comparing `tmp/fern_pushcash-0.0.3.tar.gz` & `tmp/fern_pushcash-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_pushcash-0.0.3.tar", max compression
+gzip compressed data, was "fern_pushcash-0.0.4.tar", max compression
```

## Comparing `fern_pushcash-0.0.3.tar` & `fern_pushcash-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     2498 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/README.md
--rw-r--r--   0        0        0      376 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1677 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/client.py
--rw-r--r--   0        0        0      348 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      204 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/environment.py
--rw-r--r--   0        0        0        0 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/py.typed
--rw-r--r--   0        0        0     1633 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/__init__.py
--rw-r--r--   0        0        0      499 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/__init__.py
--rw-r--r--   0        0        0     6807 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/client.py
--rw-r--r--   0        0        0      701 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/__init__.py
--rw-r--r--   0        0        0     1376 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/account_balance.py
--rw-r--r--   0        0        0      885 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/list_transactions_response.py
--rw-r--r--   0        0        0     1779 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction.py
--rw-r--r--   0        0        0     1126 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_fee_detail.py
--rw-r--r--   0        0        0      799 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_fee_type.py
--rw-r--r--   0        0        0     1001 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_source.py
--rw-r--r--   0        0        0      569 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_source_type.py
--rw-r--r--   0        0        0      600 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_status.py
--rw-r--r--   0        0        0      175 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/commons/__init__.py
--rw-r--r--   0        0        0      237 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      308 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/commons/types/currency.py
--rw-r--r--   0        0        0       78 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/commons/types/cursor.py
--rw-r--r--   0        0        0      510 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/commons/types/direction.py
--rw-r--r--   0        0        0      117 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/commons/types/error.py
--rw-r--r--   0        0        0      213 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/__init__.py
--rw-r--r--   0        0        0     5164 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/client.py
--rw-r--r--   0        0        0      299 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/types/__init__.py
--rw-r--r--   0        0        0     1357 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/types/event.py
--rw-r--r--   0        0        0      563 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/types/event_source_type.py
--rw-r--r--   0        0        0      893 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/types/event_type.py
--rw-r--r--   0        0        0      861 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/events/types/list_events_response.py
--rw-r--r--   0        0        0      233 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/__init__.py
--rw-r--r--   0        0        0     9114 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/client.py
--rw-r--r--   0        0        0      329 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/types/__init__.py
--rw-r--r--   0        0        0     1396 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/types/intent.py
--rw-r--r--   0        0        0      998 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/types/intent_failure_details.py
--rw-r--r--   0        0        0     1585 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/types/intent_status.py
--rw-r--r--   0        0        0      865 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/intent/types/list_intents_response.py
--rw-r--r--   0        0        0      199 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/transfer/__init__.py
--rw-r--r--   0        0        0     7427 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/transfer/client.py
--rw-r--r--   0        0        0      266 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/__init__.py
--rw-r--r--   0        0        0      873 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/list_transfers_response.py
--rw-r--r--   0        0        0     1239 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/transfer.py
--rw-r--r--   0        0        0      656 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/transfer_status.py
--rw-r--r--   0        0        0      485 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/user/__init__.py
--rw-r--r--   0        0        0     9386 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/user/client.py
--rw-r--r--   0        0        0      683 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/user/types/__init__.py
--rw-r--r--   0        0        0      892 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/user/types/kyc.py
--rw-r--r--   0        0        0      320 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/user/types/kyc_method.py
--rw-r--r--   0        0        0      857 2023-07-05 19:31:27.195769 fern_pushcash-0.0.3/src/pushcash/resources/user/types/list_users_response.py
--rw-r--r--   0        0        0     1335 2023-07-05 19:31:27.199771 fern_pushcash-0.0.3/src/pushcash/resources/user/types/payment_credential.py
--rw-r--r--   0        0        0      917 2023-07-05 19:31:27.199771 fern_pushcash-0.0.3/src/pushcash/resources/user/types/payment_credential_account.py
--rw-r--r--   0        0        0      939 2023-07-05 19:31:27.199771 fern_pushcash-0.0.3/src/pushcash/resources/user/types/payment_credential_card.py
--rw-r--r--   0        0        0      508 2023-07-05 19:31:27.199771 fern_pushcash-0.0.3/src/pushcash/resources/user/types/update_user_request_status.py
--rw-r--r--   0        0        0     1499 2023-07-05 19:31:27.199771 fern_pushcash-0.0.3/src/pushcash/resources/user/types/user.py
--rw-r--r--   0        0        0      810 2023-07-05 19:31:27.199771 fern_pushcash-0.0.3/src/pushcash/resources/user/types/user_status.py
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 fern_pushcash-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2498 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/README.md
+-rw-r--r--   0        0        0      376 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1677 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/client.py
+-rw-r--r--   0        0        0      348 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      204 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/environment.py
+-rw-r--r--   0        0        0        0 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/py.typed
+-rw-r--r--   0        0        0     1633 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/__init__.py
+-rw-r--r--   0        0        0      499 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/__init__.py
+-rw-r--r--   0        0        0     6807 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/client.py
+-rw-r--r--   0        0        0      701 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/__init__.py
+-rw-r--r--   0        0        0     1376 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/account_balance.py
+-rw-r--r--   0        0        0      885 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/list_transactions_response.py
+-rw-r--r--   0        0        0     1779 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction.py
+-rw-r--r--   0        0        0     1126 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_fee_detail.py
+-rw-r--r--   0        0        0      799 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_fee_type.py
+-rw-r--r--   0        0        0     1001 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_source.py
+-rw-r--r--   0        0        0      569 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_source_type.py
+-rw-r--r--   0        0        0      600 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_status.py
+-rw-r--r--   0        0        0      175 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/commons/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      308 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/commons/types/currency.py
+-rw-r--r--   0        0        0       78 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/commons/types/cursor.py
+-rw-r--r--   0        0        0      510 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/commons/types/direction.py
+-rw-r--r--   0        0        0      117 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/commons/types/error.py
+-rw-r--r--   0        0        0      213 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/__init__.py
+-rw-r--r--   0        0        0     5164 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/client.py
+-rw-r--r--   0        0        0      299 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/types/__init__.py
+-rw-r--r--   0        0        0     1357 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/types/event.py
+-rw-r--r--   0        0        0      563 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/types/event_source_type.py
+-rw-r--r--   0        0        0      893 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/types/event_type.py
+-rw-r--r--   0        0        0      861 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/events/types/list_events_response.py
+-rw-r--r--   0        0        0      233 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/__init__.py
+-rw-r--r--   0        0        0     9114 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/client.py
+-rw-r--r--   0        0        0      329 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/types/__init__.py
+-rw-r--r--   0        0        0     1396 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/types/intent.py
+-rw-r--r--   0        0        0      998 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/types/intent_failure_details.py
+-rw-r--r--   0        0        0     1585 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/types/intent_status.py
+-rw-r--r--   0        0        0      865 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/intent/types/list_intents_response.py
+-rw-r--r--   0        0        0      199 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/transfer/__init__.py
+-rw-r--r--   0        0        0     7427 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/transfer/client.py
+-rw-r--r--   0        0        0      266 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/__init__.py
+-rw-r--r--   0        0        0      873 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/list_transfers_response.py
+-rw-r--r--   0        0        0     1239 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/transfer.py
+-rw-r--r--   0        0        0      656 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/transfer_status.py
+-rw-r--r--   0        0        0      485 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/__init__.py
+-rw-r--r--   0        0        0     9386 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/client.py
+-rw-r--r--   0        0        0      683 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/__init__.py
+-rw-r--r--   0        0        0      892 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/kyc.py
+-rw-r--r--   0        0        0      320 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/kyc_method.py
+-rw-r--r--   0        0        0      857 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/list_users_response.py
+-rw-r--r--   0        0        0     1335 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/payment_credential.py
+-rw-r--r--   0        0        0      917 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/payment_credential_account.py
+-rw-r--r--   0        0        0      939 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/payment_credential_card.py
+-rw-r--r--   0        0        0      508 2023-07-05 19:50:06.228596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/update_user_request_status.py
+-rw-r--r--   0        0        0     1499 2023-07-05 19:50:06.232596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/user.py
+-rw-r--r--   0        0        0      810 2023-07-05 19:50:06.232596 fern_pushcash-0.0.4/src/pushcash/resources/user/types/user_status.py
+-rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 fern_pushcash-0.0.4/PKG-INFO
```

### Comparing `fern_pushcash-0.0.3/README.md` & `fern_pushcash-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/__init__.py` & `fern_pushcash-0.0.4/src/pushcash/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/client.py` & `fern_pushcash-0.0.4/src/pushcash/client.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/core/datetime_utils.py` & `fern_pushcash-0.0.4/src/pushcash/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/core/jsonable_encoder.py` & `fern_pushcash-0.0.4/src/pushcash/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/__init__.py` & `fern_pushcash-0.0.4/src/pushcash/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/client.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/client.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/__init__.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/account_balance.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/account_balance.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/list_transactions_response.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/list_transactions_response.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_fee_detail.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_fee_detail.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_fee_type.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_fee_type.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_source.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_source.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_source_type.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_source_type.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/balance/types/transaction_status.py` & `fern_pushcash-0.0.4/src/pushcash/resources/balance/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/events/client.py` & `fern_pushcash-0.0.4/src/pushcash/resources/events/client.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/events/types/event.py` & `fern_pushcash-0.0.4/src/pushcash/resources/events/types/event.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/events/types/event_source_type.py` & `fern_pushcash-0.0.4/src/pushcash/resources/events/types/event_source_type.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/events/types/event_type.py` & `fern_pushcash-0.0.4/src/pushcash/resources/events/types/event_type.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/events/types/list_events_response.py` & `fern_pushcash-0.0.4/src/pushcash/resources/events/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/intent/client.py` & `fern_pushcash-0.0.4/src/pushcash/resources/intent/client.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/intent/types/intent.py` & `fern_pushcash-0.0.4/src/pushcash/resources/intent/types/intent.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/intent/types/intent_failure_details.py` & `fern_pushcash-0.0.4/src/pushcash/resources/intent/types/intent_failure_details.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/intent/types/intent_status.py` & `fern_pushcash-0.0.4/src/pushcash/resources/intent/types/intent_status.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/intent/types/list_intents_response.py` & `fern_pushcash-0.0.4/src/pushcash/resources/intent/types/list_intents_response.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/transfer/client.py` & `fern_pushcash-0.0.4/src/pushcash/resources/transfer/client.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/list_transfers_response.py` & `fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/list_transfers_response.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/transfer.py` & `fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/transfer.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/transfer/types/transfer_status.py` & `fern_pushcash-0.0.4/src/pushcash/resources/transfer/types/transfer_status.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/client.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/__init__.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/kyc.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/kyc.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/list_users_response.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/list_users_response.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/payment_credential.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/payment_credential.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/payment_credential_account.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/payment_credential_account.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/payment_credential_card.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/payment_credential_card.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/user.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/user.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/src/pushcash/resources/user/types/user_status.py` & `fern_pushcash-0.0.4/src/pushcash/resources/user/types/user_status.py`

 * *Files identical despite different names*

### Comparing `fern_pushcash-0.0.3/PKG-INFO` & `fern_pushcash-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fern-pushcash
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

