# Comparing `tmp/vonage-3.7.1.tar.gz` & `tmp/vonage-4.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-3.7.1.tar", last modified: Thu Jul  6 14:03:24 2023, max compression
+gzip compressed data, was "vonage-4.0.0b0.tar", last modified: Fri Dec  2 21:31:53 2022, max compression
```

## Comparing `vonage-3.7.1.tar` & `vonage-4.0.0b0.tar`

### file list

```diff
@@ -1,186 +1,93 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.431481 vonage-3.7.1/
--rw-r--r--   0 mkahan     (503) staff       (20)      136 2023-07-06 13:17:32.000000 vonage-3.7.1/.bumpversion.cfg
--rw-r--r--   0 mkahan     (503) staff       (20)      433 2022-06-30 14:46:58.000000 vonage-3.7.1/.editorconfig
--rw-r--r--   0 mkahan     (503) staff       (20)      122 2022-06-30 15:07:43.000000 vonage-3.7.1/.pyup.yml
--rw-r--r--   0 mkahan     (503) staff       (20)     8174 2023-07-06 13:17:06.000000 vonage-3.7.1/CHANGES.md
--rw-r--r--   0 mkahan     (503) staff       (20)    10719 2022-06-30 14:46:58.000000 vonage-3.7.1/LICENSE.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      408 2022-06-30 14:46:58.000000 vonage-3.7.1/MANIFEST.in
--rw-r--r--   0 mkahan     (503) staff       (20)      473 2023-06-22 13:48:53.000000 vonage-3.7.1/Makefile
--rw-r--r--   0 mkahan     (503) staff       (20)    35404 2023-07-06 14:03:24.431596 vonage-3.7.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)    34751 2023-06-22 14:49:14.000000 vonage-3.7.1/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)       92 2023-07-06 14:01:21.000000 vonage-3.7.1/requirements.txt
--rw-r--r--   0 mkahan     (503) staff       (20)      314 2023-07-06 14:03:24.432082 vonage-3.7.1/setup.cfg
--rw-r--r--   0 mkahan     (503) staff       (20)     1204 2023-07-06 13:45:06.000000 vonage-3.7.1/setup.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.334503 vonage-3.7.1/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.357143 vonage-3.7.1/src/vonage/
--rw-r--r--   0 mkahan     (503) staff       (20)       78 2023-07-06 13:17:32.000000 vonage-3.7.1/src/vonage/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      998 2023-06-22 14:49:14.000000 vonage-3.7.1/src/vonage/_internal.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3823 2023-01-22 18:24:31.000000 vonage-3.7.1/src/vonage/account.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5461 2023-01-22 18:20:49.000000 vonage-3.7.1/src/vonage/application.py
--rw-r--r--   0 mkahan     (503) staff       (20)    16028 2023-06-30 15:28:23.000000 vonage-3.7.1/src/vonage/client.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1094 2023-06-22 14:49:14.000000 vonage-3.7.1/src/vonage/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6493 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/meetings.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4597 2023-06-22 14:49:14.000000 vonage-3.7.1/src/vonage/messages.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.363331 vonage-3.7.1/src/vonage/ncco_builder/
--rw-r--r--   0 mkahan     (503) staff       (20)       20 2023-02-09 17:41:54.000000 vonage-3.7.1/src/vonage/ncco_builder/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1656 2023-07-06 03:31:31.000000 vonage-3.7.1/src/vonage/ncco_builder/connect_endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)      799 2023-07-06 03:31:31.000000 vonage-3.7.1/src/vonage/ncco_builder/input_types.py
--rw-r--r--   0 mkahan     (503) staff       (20)     8430 2023-07-06 03:31:31.000000 vonage-3.7.1/src/vonage/ncco_builder/ncco.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1747 2023-07-06 03:31:31.000000 vonage-3.7.1/src/vonage/ncco_builder/pay_prompts.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1282 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/number_insight.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1108 2023-06-06 18:21:48.000000 vonage-3.7.1/src/vonage/number_management.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6954 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/proactive_connect.py
--rw-r--r--   0 mkahan     (503) staff       (20)      986 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/redact.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1077 2023-01-22 18:16:31.000000 vonage-3.7.1/src/vonage/short_codes.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1798 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/sms.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4792 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/subaccounts.py
--rw-r--r--   0 mkahan     (503) staff       (20)      480 2023-04-14 16:57:16.000000 vonage-3.7.1/src/vonage/ussd.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1571 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/verify.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4001 2023-07-06 03:31:31.000000 vonage-3.7.1/src/vonage/verify2.py
--rw-r--r--   0 mkahan     (503) staff       (20)     3418 2023-06-22 13:48:53.000000 vonage-3.7.1/src/vonage/voice.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.360453 vonage-3.7.1/src/vonage.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)    35404 2023-07-06 14:03:24.000000 vonage-3.7.1/src/vonage.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     6252 2023-07-06 14:03:24.000000 vonage-3.7.1/src/vonage.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2023-07-06 14:03:24.000000 vonage-3.7.1/src/vonage.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       79 2023-07-06 14:03:24.000000 vonage-3.7.1/src/vonage.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        7 2023-07-06 14:03:24.000000 vonage-3.7.1/src/vonage.egg-info/top_level.txt
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.377738 vonage-3.7.1/tests/
--rw-r--r--   0 mkahan     (503) staff       (20)     2602 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/conftest.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.379633 vonage-3.7.1/tests/data/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.336036 vonage-3.7.1/tests/data/account/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.384049 vonage-3.7.1/tests/data/account/secret_management/
--rw-r--r--   0 mkahan     (503) staff       (20)      350 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/create-validation.json
--rw-r--r--   0 mkahan     (503) staff       (20)      210 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/create.json
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/delete.json
--rw-r--r--   0 mkahan     (503) staff       (20)      210 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/get.json
--rw-r--r--   0 mkahan     (503) staff       (20)      303 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/last-secret.json
--rw-r--r--   0 mkahan     (503) staff       (20)      394 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/list.json
--rw-r--r--   0 mkahan     (503) staff       (20)      286 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/max-secrets.json
--rw-r--r--   0 mkahan     (503) staff       (20)      225 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/missing.json
--rw-r--r--   0 mkahan     (503) staff       (20)      217 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/account/secret_management/unauthorized.json
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.387747 vonage-3.7.1/tests/data/applications/
--rw-r--r--   0 mkahan     (503) staff       (20)      423 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/applications/create_application.json
--rw-r--r--   0 mkahan     (503) staff       (20)      323 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/applications/get_application.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1057 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/applications/list_applications.json
--rw-r--r--   0 mkahan     (503) staff       (20)      317 2022-07-07 13:48:10.000000 vonage-3.7.1/tests/data/applications/update_application.json
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.402531 vonage-3.7.1/tests/data/meetings/
--rw-r--r--   0 mkahan     (503) staff       (20)       93 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/delete_recording_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      187 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/delete_theme_in_use.json
--rw-r--r--   0 mkahan     (503) staff       (20)        2 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/empty_themes.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1880 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/get_recording.json
--rw-r--r--   0 mkahan     (503) staff       (20)      116 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/get_recording_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)     2101 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/get_session_recordings.json
--rw-r--r--   0 mkahan     (503) staff       (20)      131 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/get_session_recordings_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      227 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/list_dial_in_numbers.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1888 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/list_logo_upload_urls.json
--rw-r--r--   0 mkahan     (503) staff       (20)      152 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/list_rooms_theme_id_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)     2193 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/list_rooms_with_theme_id.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1078 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/list_themes.json
--rw-r--r--   0 mkahan     (503) staff       (20)      210 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/logo_key_error.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1289 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/long_term_room.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1366 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/long_term_room_with_theme.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1320 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/meeting_room.json
--rw-r--r--   0 mkahan     (503) staff       (20)     3685 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/multiple_fewer_rooms.json
--rw-r--r--   0 mkahan     (503) staff       (20)     8420 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/multiple_rooms.json
--rw-r--r--   0 mkahan     (503) staff       (20)      463 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/theme.json
--rw-r--r--   0 mkahan     (503) staff       (20)      109 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/theme_name_in_use.json
--rw-r--r--   0 mkahan     (503) staff       (20)      126 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/theme_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)       88 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/unauthorized.json
--rw-r--r--   0 mkahan     (503) staff       (20)      144 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/update_application_theme.json
--rw-r--r--   0 mkahan     (503) staff       (20)      146 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/update_application_theme_id_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      119 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/update_no_keys.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1292 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/update_room.json
--rw-r--r--   0 mkahan     (503) staff       (20)      177 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/update_room_type_error.json
--rw-r--r--   0 mkahan     (503) staff       (20)      109 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/update_theme_already_exists.json
--rw-r--r--   0 mkahan     (503) staff       (20)      490 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/meetings/updated_theme.json
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/no_content.json
--rw-r--r--   0 mkahan     (503) staff       (20)        0 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/null.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1704 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/private_key.txt
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.411467 vonage-3.7.1/tests/data/proactive_connect/
--rw-r--r--   0 mkahan     (503) staff       (20)      340 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/create_list_400.json
--rw-r--r--   0 mkahan     (503) staff       (20)      391 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/create_list_basic.json
--rw-r--r--   0 mkahan     (503) staff       (20)      618 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/create_list_manual.json
--rw-r--r--   0 mkahan     (503) staff       (20)      770 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/create_list_salesforce.json
--rw-r--r--   0 mkahan     (503) staff       (20)      206 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/fetch_list_400.json
--rw-r--r--   0 mkahan     (503) staff       (20)      618 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/get_list.json
--rw-r--r--   0 mkahan     (503) staff       (20)      308 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/item.json
--rw-r--r--   0 mkahan     (503) staff       (20)      247 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/item_400.json
--rw-r--r--   0 mkahan     (503) staff       (20)      197 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/list_404.json
--rw-r--r--   0 mkahan     (503) staff       (20)     1336 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/list_all_items.json
--rw-r--r--   0 mkahan     (503) staff       (20)     2728 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/list_events.json
--rw-r--r--   0 mkahan     (503) staff       (20)     2661 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/list_lists.json
--rw-r--r--   0 mkahan     (503) staff       (20)      197 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      310 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/update_item.json
--rw-r--r--   0 mkahan     (503) staff       (20)      646 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/update_list.json
--rw-r--r--   0 mkahan     (503) staff       (20)      678 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/update_list_salesforce.json
--rw-r--r--   0 mkahan     (503) staff       (20)       21 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/proactive_connect/upload_from_csv.json
--rw-r--r--   0 mkahan     (503) staff       (20)      451 2022-06-30 14:46:58.000000 vonage-3.7.1/tests/data/public_key.txt
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.420065 vonage-3.7.1/tests/data/subaccounts/
--rw-r--r--   0 mkahan     (503) staff       (20)      387 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/balance_transfer.json
--rw-r--r--   0 mkahan     (503) staff       (20)      385 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/credit_transfer.json
--rw-r--r--   0 mkahan     (503) staff       (20)      249 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/forbidden.json
--rw-r--r--   0 mkahan     (503) staff       (20)      228 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/insufficient_credit.json
--rw-r--r--   0 mkahan     (503) staff       (20)      223 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/invalid_credentials.json
--rw-r--r--   0 mkahan     (503) staff       (20)      326 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/invalid_number_transfer.json
--rw-r--r--   0 mkahan     (503) staff       (20)      270 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/invalid_transfer.json
--rw-r--r--   0 mkahan     (503) staff       (20)      755 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/list_balance_transfers.json
--rw-r--r--   0 mkahan     (503) staff       (20)      760 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/list_credit_transfers.json
--rw-r--r--   0 mkahan     (503) staff       (20)      859 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/list_subaccounts.json
--rw-r--r--   0 mkahan     (503) staff       (20)      262 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/modified_subaccount.json
--rw-r--r--   0 mkahan     (503) staff       (20)      399 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/must_be_number.json
--rw-r--r--   0 mkahan     (503) staff       (20)      234 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      307 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/number_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      398 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/same_from_and_to_accounts.json
--rw-r--r--   0 mkahan     (503) staff       (20)      288 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/subaccount.json
--rw-r--r--   0 mkahan     (503) staff       (20)      133 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/transfer_number.json
--rw-r--r--   0 mkahan     (503) staff       (20)      355 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/transfer_validation_error.json
--rw-r--r--   0 mkahan     (503) staff       (20)      476 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/subaccounts/validation_error.json
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.421387 vonage-3.7.1/tests/data/verify/
--rw-r--r--   0 mkahan     (503) staff       (20)      115 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/verify/blocked_with_network.json
--rw-r--r--   0 mkahan     (503) staff       (20)      139 2022-08-30 16:27:52.000000 vonage-3.7.1/tests/data/verify/blocked_with_network_and_request_id.json
--rw-r--r--   0 mkahan     (503) staff       (20)      121 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/data/verify/blocked_with_request_id.json
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.427814 vonage-3.7.1/tests/data/verify2/
--rw-r--r--   0 mkahan     (503) staff       (20)      259 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/already_verified.json
--rw-r--r--   0 mkahan     (503) staff       (20)       87 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/check_code.json
--rw-r--r--   0 mkahan     (503) staff       (20)      221 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/code_not_supported.json
--rw-r--r--   0 mkahan     (503) staff       (20)       59 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/create_request.json
--rw-r--r--   0 mkahan     (503) staff       (20)      294 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/error_conflict.json
--rw-r--r--   0 mkahan     (503) staff       (20)      227 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/fraud_check_invalid_account.json
--rw-r--r--   0 mkahan     (503) staff       (20)      227 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/invalid_code.json
--rw-r--r--   0 mkahan     (503) staff       (20)      364 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/invalid_email.json
--rw-r--r--   0 mkahan     (503) staff       (20)      207 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/invalid_sender.json
--rw-r--r--   0 mkahan     (503) staff       (20)      208 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/rate_limit.json
--rw-r--r--   0 mkahan     (503) staff       (20)      259 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/request_not_found.json
--rw-r--r--   0 mkahan     (503) staff       (20)      236 2023-06-20 15:43:03.000000 vonage-3.7.1/tests/data/verify2/too_many_code_attempts.json
--rw-r--r--   0 mkahan     (503) staff       (20)     7290 2022-12-14 19:26:19.000000 vonage-3.7.1/tests/test_account.py
--rw-r--r--   0 mkahan     (503) staff       (20)     8355 2022-07-27 14:58:22.000000 vonage-3.7.1/tests/test_application.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1216 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_client.py
--rw-r--r--   0 mkahan     (503) staff       (20)      401 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_getters_setters.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2190 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_jwt.py
--rw-r--r--   0 mkahan     (503) staff       (20)    26664 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_meetings.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1342 2023-03-14 18:56:29.000000 vonage-3.7.1/tests/test_messages_send_message.py
--rw-r--r--   0 mkahan     (503) staff       (20)     9147 2023-03-14 18:56:29.000000 vonage-3.7.1/tests/test_messages_validate_input.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.430380 vonage-3.7.1/tests/test_ncco_builder/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2023-07-06 14:03:24.431133 vonage-3.7.1/tests/test_ncco_builder/ncco_samples/
--rw-r--r--   0 mkahan     (503) staff       (20)     4789 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_ncco_builder/ncco_samples/ncco_action_samples.py
--rw-r--r--   0 mkahan     (503) staff       (20)     4702 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_ncco_builder/ncco_samples/ncco_builder_samples.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2254 2023-01-16 01:40:10.000000 vonage-3.7.1/tests/test_ncco_builder/test_connect_endpoints.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1447 2023-01-16 01:40:10.000000 vonage-3.7.1/tests/test_ncco_builder/test_input_types.py
--rw-r--r--   0 mkahan     (503) staff       (20)    10362 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_ncco_builder/test_ncco_actions.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1062 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_ncco_builder/test_ncco_builder.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1879 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_ncco_builder/test_pay_prompts.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1975 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_number_insight.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1912 2023-03-14 18:56:29.000000 vonage-3.7.1/tests/test_number_management.py
--rw-r--r--   0 mkahan     (503) staff       (20)      427 2023-02-09 17:40:54.000000 vonage-3.7.1/tests/test_packages.py
--rw-r--r--   0 mkahan     (503) staff       (20)    20857 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_proactive_connect.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1087 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_redact.py
--rw-r--r--   0 mkahan     (503) staff       (20)     5263 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_rest_calls.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2221 2022-07-27 14:58:22.000000 vonage-3.7.1/tests/test_short_codes.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2616 2023-02-28 14:58:56.000000 vonage-3.7.1/tests/test_signature.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1549 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_sms.py
--rw-r--r--   0 mkahan     (503) staff       (20)    25301 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_subaccounts.py
--rw-r--r--   0 mkahan     (503) staff       (20)      985 2022-07-05 17:10:38.000000 vonage-3.7.1/tests/test_ussd.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6741 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_verify.py
--rw-r--r--   0 mkahan     (503) staff       (20)    17583 2023-06-22 14:49:14.000000 vonage-3.7.1/tests/test_verify2.py
--rw-r--r--   0 mkahan     (503) staff       (20)     6782 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/test_voice.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1564 2023-06-22 13:48:53.000000 vonage-3.7.1/tests/util.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.809967 vonage-4.0.0b0/
+-rw-r--r--   0 mkahan     (503) staff       (20)      138 2022-12-02 21:30:01.000000 vonage-4.0.0b0/.bumpversion.cfg
+-rw-r--r--   0 mkahan     (503) staff       (20)      433 2022-06-30 14:46:58.000000 vonage-4.0.0b0/.editorconfig
+-rw-r--r--   0 mkahan     (503) staff       (20)      122 2022-06-30 15:07:43.000000 vonage-4.0.0b0/.pyup.yml
+-rw-r--r--   0 mkahan     (503) staff       (20)     6091 2022-12-01 15:20:15.000000 vonage-4.0.0b0/CHANGES.md
+-rw-r--r--   0 mkahan     (503) staff       (20)    10719 2022-06-30 14:46:58.000000 vonage-4.0.0b0/LICENSE.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      408 2022-06-30 14:46:58.000000 vonage-4.0.0b0/MANIFEST.in
+-rw-r--r--   0 mkahan     (503) staff       (20)      453 2022-12-01 15:20:15.000000 vonage-4.0.0b0/Makefile
+-rw-r--r--   0 mkahan     (503) staff       (20)    22663 2022-12-02 21:31:53.810095 vonage-4.0.0b0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)    22008 2022-08-02 15:43:34.000000 vonage-4.0.0b0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)       71 2022-12-01 15:20:15.000000 vonage-4.0.0b0/requirements.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      314 2022-12-02 21:31:53.811231 vonage-4.0.0b0/setup.cfg
+-rw-r--r--   0 mkahan     (503) staff       (20)     1183 2022-12-02 21:30:01.000000 vonage-4.0.0b0/setup.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.748084 vonage-4.0.0b0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.764603 vonage-4.0.0b0/src/vonage/
+-rw-r--r--   0 mkahan     (503) staff       (20)       47 2022-12-02 21:30:01.000000 vonage-4.0.0b0/src/vonage/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      608 2022-12-02 02:30:34.000000 vonage-4.0.0b0/src/vonage/_internal.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3823 2022-12-02 02:37:38.000000 vonage-4.0.0b0/src/vonage/account.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5461 2022-12-02 02:34:11.000000 vonage-4.0.0b0/src/vonage/application.py
+-rw-r--r--   0 mkahan     (503) staff       (20)    15031 2022-12-02 21:26:00.000000 vonage-4.0.0b0/src/vonage/client.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      947 2022-12-02 21:26:00.000000 vonage-4.0.0b0/src/vonage/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3780 2022-12-02 02:36:36.000000 vonage-4.0.0b0/src/vonage/messages.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1282 2022-12-02 02:33:39.000000 vonage-4.0.0b0/src/vonage/number_insight.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1184 2022-12-02 02:33:52.000000 vonage-4.0.0b0/src/vonage/numbers.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      986 2022-12-02 02:35:03.000000 vonage-4.0.0b0/src/vonage/redact.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1077 2022-12-02 02:30:27.000000 vonage-4.0.0b0/src/vonage/short_codes.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1798 2022-12-02 02:37:10.000000 vonage-4.0.0b0/src/vonage/sms.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      480 2022-12-01 16:44:54.000000 vonage-4.0.0b0/src/vonage/ussd.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1538 2022-12-02 02:36:54.000000 vonage-4.0.0b0/src/vonage/verify.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     9271 2022-12-02 21:26:00.000000 vonage-4.0.0b0/src/vonage/video.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     3340 2022-12-02 02:34:37.000000 vonage-4.0.0b0/src/vonage/voice.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.769233 vonage-4.0.0b0/src/vonage.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)    22663 2022-12-02 21:31:53.000000 vonage-4.0.0b0/src/vonage.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2379 2022-12-02 21:31:53.000000 vonage-4.0.0b0/src/vonage.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2022-12-02 21:31:53.000000 vonage-4.0.0b0/src/vonage.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       61 2022-12-02 21:31:53.000000 vonage-4.0.0b0/src/vonage.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        7 2022-12-02 21:31:53.000000 vonage-4.0.0b0/src/vonage.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.786084 vonage-4.0.0b0/tests/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2097 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/conftest.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.786680 vonage-4.0.0b0/tests/data/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.749054 vonage-4.0.0b0/tests/data/account/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.789047 vonage-4.0.0b0/tests/data/account/secret_management/
+-rw-r--r--   0 mkahan     (503) staff       (20)      350 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/create-validation.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      210 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/create.json
+-rw-r--r--   0 mkahan     (503) staff       (20)        0 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/delete.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      210 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/get.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      303 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/last-secret.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      394 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/list.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      286 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/max-secrets.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      225 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/missing.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      217 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/account/secret_management/unauthorized.json
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.790464 vonage-4.0.0b0/tests/data/applications/
+-rw-r--r--   0 mkahan     (503) staff       (20)      423 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/applications/create_application.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      323 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/applications/get_application.json
+-rw-r--r--   0 mkahan     (503) staff       (20)     1057 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/applications/list_applications.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      317 2022-07-07 13:48:10.000000 vonage-4.0.0b0/tests/data/applications/update_application.json
+-rw-r--r--   0 mkahan     (503) staff       (20)     1704 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/private_key.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)      451 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/data/public_key.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.793699 vonage-4.0.0b0/tests/data/rest_calls/
+-rw-r--r--   0 mkahan     (503) staff       (20)       52 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/rest_calls/patch.json
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.799045 vonage-4.0.0b0/tests/data/verify/
+-rw-r--r--   0 mkahan     (503) staff       (20)      115 2022-08-30 16:27:52.000000 vonage-4.0.0b0/tests/data/verify/blocked_with_network.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      139 2022-08-30 16:27:52.000000 vonage-4.0.0b0/tests/data/verify/blocked_with_network_and_request_id.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      121 2022-08-30 16:27:52.000000 vonage-4.0.0b0/tests/data/verify/blocked_with_request_id.json
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2022-12-02 21:31:53.809436 vonage-4.0.0b0/tests/data/video/
+-rw-r--r--   0 mkahan     (503) staff       (20)      411 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/create_archive.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      636 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/create_session.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      177 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/disable_mute_multiple_streams.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      587 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/get_archive.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      140 2022-12-02 21:25:16.000000 vonage-4.0.0b0/tests/data/video/get_stream.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      709 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/list_archives.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      219 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/list_streams.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      177 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/mute_multiple_streams.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      177 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/mute_specific_stream.json
+-rw-r--r--   0 mkahan     (503) staff       (20)      380 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/data/video/stop_archive.json
+-rw-r--r--   0 mkahan     (503) staff       (20)     7290 2022-12-01 15:20:15.000000 vonage-4.0.0b0/tests/test_account.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     8355 2022-07-27 14:58:22.000000 vonage-4.0.0b0/tests/test_application.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1403 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/test_client.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      627 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/test_getters_setters.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1345 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/test_messages_send_message.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     4057 2022-06-30 14:46:58.000000 vonage-4.0.0b0/tests/test_messages_validate_input.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1975 2022-07-27 14:58:22.000000 vonage-4.0.0b0/tests/test_number_insight.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1912 2022-07-27 14:58:22.000000 vonage-4.0.0b0/tests/test_numbers.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1087 2022-07-27 14:58:22.000000 vonage-4.0.0b0/tests/test_redact.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5008 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/test_rest_calls.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2221 2022-07-27 14:58:22.000000 vonage-4.0.0b0/tests/test_short_codes.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2616 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/test_signature.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1549 2022-07-27 14:58:22.000000 vonage-4.0.0b0/tests/test_sms.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      985 2022-07-05 17:10:38.000000 vonage-4.0.0b0/tests/test_ussd.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     6741 2022-11-24 04:04:31.000000 vonage-4.0.0b0/tests/test_verify.py
+-rw-r--r--   0 mkahan     (503) staff       (20)    14086 2022-12-02 21:26:00.000000 vonage-4.0.0b0/tests/test_video.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     5805 2022-08-09 12:53:58.000000 vonage-4.0.0b0/tests/test_voice.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1613 2022-11-06 18:20:01.000000 vonage-4.0.0b0/tests/util.py
```

### Comparing `vonage-3.7.1/CHANGES.md` & `vonage-4.0.0b0/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,7 @@
-# 3.7.1
-- Fixing dependency version to a specific major version
-
-# 3.7.0
-- Adding support for the [Vonage Meetings API](https://developer.vonage.com/en/meetings/overview)
-- Adding partial support for the [Vonage Proactive Connect API](https://developer.vonage.com/en/proactive-connect/overview) - supporting API methods relating to `lists`, `items` and `events`
-- Returning a more descriptive (non-internal) error message if invalid values are provided for `application_id` and/or `private_key` when instantiating a Vonage client object
-
-# 3.6.0
-- Adding support for the [Vonage Subaccounts API](https://developer.vonage.com/en/account/subaccounts/overview)
-
-# 3.5.2
-- Using the [Vonage JWT Generator](https://github.com/Vonage/vonage-python-jwt) instead of `PyJWT` for generating JWTs.
-- Other internal refactoring and enhancements
-
-# 3.5.1
-- Updating the internal use of the `fraud_check` parameter in the Vonage Verify V2 API
-
-# 3.5.0
-- Adding support for V2 of the Vonage Verify API
-    - Multiple authentication channels are supported (sms, voice, email, whatsapp, whatsapp interactive messages and silent authentication)
-    - Using fallback channels is now possible in case verification methods fail
-    - You can now customise the verification code that is sent, or even specify your own custom code
-- Adding `advancedMachineDetection` functionality to the NCCO builder for the Vonage Voice API
-
-# 3.4.0
-- Internal refactoring changes
-- Using header authentication for the Numbers API
-
-# 3.3.0
-- Updated Messages API:
-    - Added new messaging channels for Viber Service Messages (`video`, `file`)
-    - Added new WhatsApp `sticker` message channel
-    - Increased `client_ref` max value to 100 characters
-- Deprecated `pay` action in the NCCO builder as it is being removed by Vonage
-
-# 3.2.2
-- Fixing a bug on Windows
-
-# 3.2.1
-- Fixing an import bug
-
-# 3.2.0
-- Adding an NCCO Builder to make it easier to work with NCCOs when using the Voice API
-- Individual NCCO Actions can be created as Pydantic models, which can be built into an NCCO via the `Ncco.build_ncco` method
-
 # 3.1.0
 - Supporting Python 3.11
 - Upgrading some old dependencies
 
 # 3.0.2
 - Bugfix in `messages.py` where authentication method was not being checked for correctly, throwing an error when using header auth.
```

### Comparing `vonage-3.7.1/LICENSE.txt` & `vonage-4.0.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/PKG-INFO` & `vonage-4.0.0b0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,32 @@
-Metadata-Version: 2.1
-Name: vonage
-Version: 3.7.1
-Summary: Vonage Server SDK for Python
-Home-page: https://github.com/Vonage/vonage-python-sdk
-Author: Vonage
-Author-email: devrel@vonage.com
-License: Apache
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Vonage Server SDK for Python
 
 <img src="https://developer.nexmo.com/assets/images/Vonage_Nexmo.svg" height="48px" alt="Nexmo is now known as Vonage" />
 
 [![PyPI version](https://badge.fury.io/py/vonage.svg)](https://badge.fury.io/py/vonage)
 [![Build Status](https://github.com/Vonage/vonage-python-sdk/workflows/Build/badge.svg)](https://github.com/Vonage/vonage-python-sdk/actions)
+[![codecov](https://codecov.io/gh/Vonage/vonage-python-sdk/branch/master/graph/badge.svg)](https://codecov.io/gh/Vonage/vonage-python-sdk)
 [![Python versions supported](https://img.shields.io/pypi/pyversions/vonage.svg)](https://pypi.python.org/pypi/vonage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 This is the Python server SDK for Vonage's API. To use it you'll
 need a Vonage account. Sign up [for free at vonage.com][signup].
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [SMS API](#sms-api)
 - [Messages API](#messages-api)
 - [Voice API](#voice-api)
-- [NCCO Builder](#ncco-builder)
-- [Verify V2 API](#verify-v2-api)
-- [Verify V1 API](#verify-v1-api)
-- [Meetings API](#meetings-api)
+- [Verify API](#verify-api)
 - [Number Insight API](#number-insight-api)
-- [Proactive Connect API](#proactive-connect-api)
-- [Account API](#account-api)
-- [Subaccounts API](#subaccounts-api)
 - [Number Management API](#number-management-api)
-- [Pricing API](#pricing-api)
 - [Managing Secrets](#managing-secrets)
 - [Application API](#application-api)
-- [Validating Webhook Signatures](#validate-webhook-signatures)
-- [JWT Parameters](#jwt-parameters)
 - [Overriding API Attributes](#overriding-api-attributes)
 - [Frequently Asked Questions](#frequently-asked-questions)
-- [Contributing](#contributing)
 - [License](#license)
 
 ## Installation
 
 To install the Python client library using pip:
 
     pip install vonage
@@ -362,146 +333,16 @@
 
 ### Get recording
 
 ```python
 response = client.get_recording(RECORDING_URL)
 ```
 
-## NCCO Builder
-
-The SDK contains a builder to help you create Call Control Objects (NCCOs) for use with the Vonage Voice API.
-
-For more information, [check the full NCCO reference documentation on the Vonage website](https://developer.vonage.com/voice/voice-api/ncco-reference).
-
-An NCCO is a list of "Actions": steps to be followed when a call is initiated or received.
-
-Use the builder to construct valid NCCO actions, which are modelled in the SDK as [Pydantic](https://docs.pydantic.dev) models, and build them into an NCCO. The NCCO actions supported by the builder are:
-
-* Record
-* Conversation
-* Connect
-* Talk
-* Stream
-* Input
-* Notify
-
-### Construct actions
-
-```python
-record = Ncco.Record(eventUrl=['https://example.com'])
-talk = Ncco.Talk(text='Hello from Vonage!', bargeIn=True, loop=5, premium=True)
-```
-
-The Connect action has each valid endpoint type (phone, application, WebSocket, SIP and VBC) specified as a Pydantic model so these can be validated, though it is also possible to pass in a dict with the endpoint properties directly into the `Ncco.Connect` object.
-
-This example shows a Connect action created with an endpoint object.
-
-```python
-phone = ConnectEndpoints.PhoneEndpoint(
-        number='447000000000',
-        dtmfAnswer='1p2p3p#**903#',
-    )
-connect = Ncco.Connect(endpoint=phone, eventUrl=['https://example.com/events'], from_='447000000000')
-```
-
-This example shows a different Connect action, created with a dictionary.
-
-```python
-connect = Ncco.Connect(endpoint={'type': 'phone', 'number': '447000000000', 'dtmfAnswer': '2p02p'}, randomFromNumber=True)
-```
-
-### Build into an NCCO
-
-Create an NCCO from the actions with the `Ncco.build_ncco` method. This will be returned as a list of dicts representing each action and can be used in calls to the Voice API.
-
-```python
-ncco = Ncco.build_ncco(record, connect, talk)
-
-response = client.voice.create_call({
-    'to': [{'type': 'phone', 'number': TO_NUMBER}],
-    'from': {'type': 'phone', 'number': VONAGE_NUMBER},
-    'ncco': ncco
-})
-
-pprint(response)
-```
-
-### Note on from_ parameter in connect action
-
-When using the `connect` action, use the parameter `from_` to specify the recipient (as `from` is a reserved keyword in Python!)
-
-## Verify V2 API
-
-V2 of the Vonage Verify API lets you send verification codes via SMS, WhatsApp, Voice and Email.
-
-You can also verify a user by WhatsApp Interactive Message or by Silent Authentication on their mobile device.
-
-### Send a verification code
-
-```python
-params = {
-    'brand': 'ACME, Inc', 
-    'workflow': [{'channel': 'sms', 'to': '447700900000'}]
-}
-verify_request = verify2.new_request(params)
-```
-
-### Use silent authentication, with email as a fallback
-
-```python
-params = {
-    'brand': 'ACME, Inc', 
-    'workflow': [
-        {'channel': 'silent_auth', 'to': '447700900000'},
-        {'channel': 'email', 'to': 'customer@example.com', 'from': 'business@example.com'}
-    ]
-}
-verify_request = verify2.new_request(params)
-```
-
-### Send a verification code with custom options, including a custom code
-
-```python
-params = {
-    'locale': 'en-gb',
-    'channel_timeout': 120,
-    'client_ref': 'my client reference',
-    'code': 'asdf1234',
-    'brand': 'ACME, Inc',
-    'workflow': [{'channel': 'sms', 'to': '447700900000', 'app_hash': 'asdfghjklqw'}],
-}
-verify_request = verify2.new_request(params)
-```
-
-### Send a verification request to a blocked network
 
-This feature is only enabled if you have requested for it to be added to your account.
-
-```python
-params = {
-    'brand': 'ACME, Inc', 
-    'fraud_check': False, 
-    'workflow': [{'channel': 'sms', 'to': '447700900000'}]
-}
-verify_request = verify2.new_request(params)
-```
-
-### Check a verification code
-
-```python
-verify2.check_code(REQUEST_ID, CODE)
-```
-
-### Cancel an ongoing verification
-
-```python
-verify2.cancel_verification(REQUEST_ID)
-```
-
-## Verify V1 API
+## Verify API
 
 ### Search for a Verification request
 
 ```python
 client = vonage.Client(key='API_KEY', secret='API_SECRET')
 
 response = client.verify.search('69e2626cbc23451fbbc02f627a959677')
@@ -597,152 +438,14 @@
 
 if response["status"] == "0":
     print("Started PSD2 verification request_id is %s" % (response["request_id"]))
 else:
     print("Error: %s" % response["error_text"])
 ```
 
-## Meetings API
-
-Full docs for the [Meetings API are available here](https://developer.vonage.com/en/meetings/overview).
-
-### Create a meeting room
-
-```python
-# Instant room
-params = {'display_name': 'my_test_room'}
-meeting = client.meetings.create_room(params)
-
-# Long term room
-params = {'display_name': 'test_long_term_room', 'type': 'long_term', 'expires_at': '2023-01-30T00:47:04+0000'}
-meeting = client.meetings.create_room(params)
-```
-
-### Get all meeting rooms
-
-```python
-client.meetings.list_rooms()
-```
-
-### Get a room by id
-
-```python
-client.meetings.get_room('MY_ROOM_ID')
-```
-
-### Update a long term room
-
-```python
-params = {
-    'update_details': {
-        "available_features": {
-            "is_recording_available": False,
-            "is_chat_available": False,
-        }
-    }
-}
-meeting = client.meetings.update_room('MY_ROOM_ID', params)
-```
-
-### Get all recordings for a session
-
-```python
-session = client.meetings.get_session_recordings('MY_SESSION_ID')
-```
-
-### Get a recording by id
-
-```python
-recording = client.meetings.get_recording('MY_RECORDING_ID')
-```
-
-### Delete a recording
-
-```python
-client.meetings.delete_recording('MY_RECORDING_ID')
-```
-
-### List dial-in numbers
-
-```python
-numbers = client.meetings.list_dial_in_numbers()
-```
-
-### Create a theme
-
-```python
-params = {
-    'theme_name': 'my_theme',
-    'main_color': '#12f64e',
-    'brand_text': 'My Company',
-    'short_company_url': 'my-company',
-}
-theme = client.meetings.create_theme(params)
-```
-
-### Add a theme to a room
-
-```python
-meetings.add_theme_to_room('MY_ROOM_ID', 'MY_THEME_ID')
-```
-
-### List themes
-
-```python
-themes = client.meetings.list_themes()
-```
-
-### Get theme information
-
-```python
-theme = client.meetings.get_theme('MY_THEME_ID')
-```
-
-### Delete a theme
-
-```python
-client.meetings.delete_theme('MY_THEME_ID')
-```
-
-### Update a theme
-
-```python
-params = {
-    'update_details': {
-        'theme_name': 'updated_theme',
-        'main_color': '#FF0000',
-        'brand_text': 'My Updated Company Name',
-        'short_company_url': 'updated_company_url',
-    }
-}
-theme = client.meetings.update_theme('MY_THEME_ID', params)
-```
-
-### List all rooms using a specified theme
-
-```python
-rooms = client.meetings.list_rooms_with_theme_id('MY_THEME_ID')
-```
-
-### Update the default theme for your application
-
-```python
-response = client.meetings.update_application_theme('MY_THEME_ID')
-```
-
-### Upload a logo to a theme
-
-```python
-response = client.meetings.upload_logo_to_theme(
-        theme_id='MY_THEME_ID',
-        path_to_image='path/to/my/image.png',
-        logo_type='white', # 'white', 'colored' or 'favicon'
-    )
-```
-
 ## Number Insight API
 
 ### Basic Number Insight
 
 ```python
 client.number_insight.get_basic_number_insight(number='447700900000')
 ```
@@ -761,260 +464,28 @@
 
 ```python
 client.number_insight.get_advanced_number_insight(number='447700900000')
 ```
 
 Docs: [https://developer.nexmo.com/api/number-insight#getNumberInsightAdvanced](https://developer.nexmo.com/api/number-insight?utm_source=DEV_REL&utm_medium=github&utm_campaign=python-client-library#getNumberInsightAdvanced)
 
-## Proactive Connect API
-
-Full documentation for the [Proactive Connect API](https://developer.vonage.com/en/proactive-connect/overview) is available here.
-
-These methods help you manage lists of contacts when using the API:
-
-### Find all lists
-```python
-client.proactive_connect.list_all_lists()
-```
-
-### Create a list
-Lists can be created manually or imported from Salesforce.
-
-```python
-params = {'name': 'my list', 'description': 'my description', 'tags': ['vip']}
-client.proactive_connect.create_list(params)
-```
-
-### Get a list
-```python
-client.proactive_connect.get_list(LIST_ID)
-```
-
-### Update a list
-```python
-params = {'name': 'my list', 'tags': ['sport', 'football']}
-client.proactive_connect.update_list(LIST_ID, params)
-```
-
-### Delete a list
-```python
-client.proactive_connect.delete_list(LIST_ID)
-```
-
-### Sync a list from an external datasource
-```python
-params = {'name': 'my list', 'tags': ['sport', 'football']}
-client.proactive_connect.sync_list_from_datasource(LIST_ID)
-```
-
-These methods help you work with individual items in a list:
-### Find all items in a list
-```python
-client.proactive_connect.list_all_items(LIST_ID)
-```
-
-### Create a new list item
-```python
-data = {'firstName': 'John', 'lastName': 'Doe', 'phone': '123456789101'}
-client.proactive_connect.create_item(LIST_ID, data)
-```
-
-### Get a list item
-```python
-client.proactive_connect.get_item(LIST_ID, ITEM_ID)
-```
-
-### Update a list item
-```python
-data = {'firstName': 'John', 'lastName': 'Doe', 'phone': '447007000000'}
-client.proactive_connect.update_item(LIST_ID, ITEM_ID, data)
-```
-
-### Delete a list item
-```python
-client.proactive_connect.delete_item(LIST_ID, ITEM_ID)
-```
-
-### Download all items in a list as a .csv file
-```python
-FILE_PATH = 'path/to/the/downloaded/file/location'
-client.proactive_connect.download_list_items(LIST_ID, FILE_PATH)
-```
-
-### Upload items from a .csv file into a list
-```python
-FILE_PATH = 'path/to/the/file/to/upload/location'
-client.proactive_connect.upload_list_items(LIST_ID, FILE_PATH)
-```
-
-This method helps you work with events emitted by the Proactive Connect API when in use:
-
-### List all events
-```python
-client.proactive_connect.list_events()
-```
-
 ## Account API
 
 ### Get your account balance
 ```python
 client.account.get_balance()
 ```
 
 ### Top up your account
 This feature is only enabled when you enable auto-reload for your account in the dashboard.
 ```python
 # trx is the reference from when auto-reload was enabled and money was added
 client.account.topup(trx=transaction_reference) 
 ```
 
-## Subaccounts API
-
-This API is used to create and configure subaccounts related to your primary account and transfer credit, balances and bought numbers between accounts.
-
-The subaccounts API is disabled by default. If you want to use subaccounts, [contact support](https://api.support.vonage.com) to have the API enabled on your account.
-
-### Get a list of all subaccounts
-
-```python
-client.subaccounts.list_subaccounts()
-```
-
-### Create a subaccount
-
-```python
-client.subaccounts.create_subaccount(name='my subaccount')
-
-# With options
-client.subaccounts.create_subaccount(
-    name='my subaccount', 
-    secret='Password123', 
-    use_primary_account_balance=False,
-)
-```
-
-### Get information about a subaccount
-
-```python
-client.subaccounts.get_subaccount(SUBACCOUNT_API_KEY)
-```
-
-### Modify a subaccount
-
-```python
-client.subaccounts.modify_subaccount(
-    SUBACCOUNT_KEY,
-    suspended=True,
-    use_primary_account_balance=False,
-    name='my modified subaccount',
-)
-```
-
-### List credit transfers between accounts
-
-All fields are optional. If `start_date` or `end_date` are used, the dates must be specified in UTC ISO 8601 format, e.g. `1970-01-01T00:00:00Z`. Don't use milliseconds.
-
-```python
-client.subaccounts.list_credit_transfers(
-    start_date='2022-03-29T14:16:56Z',
-    end_date='2023-06-12T17:20:01Z',
-    subaccount=SUBACCOUNT_API_KEY, # Use to show only the results that contain this key 
-)
-```
-
-### Transfer credit between accounts
-
-Transferring credit is only possible for postpaid accounts, i.e. accounts that can have a negative balance. For prepaid and self-serve customers, account balances can be transferred between accounts (see below).
-
-```python
-client.subaccounts.transfer_credit(
-    from_=FROM_ACCOUNT, 
-    to=TO_ACCOUNT, 
-    amount=0.50, 
-    reference='test credit transfer',
-)
-```
-
-### List balance transfers between accounts
-
-All fields are optional. If `start_date` or `end_date` are used, the dates must be specified in UTC ISO 8601 format, e.g. `1970-01-01T00:00:00Z`. Don't use milliseconds.
-
-```python
-client.subaccounts.list_balance_transfers(
-    start_date='2022-03-29T14:16:56Z',
-    end_date='2023-06-12T17:20:01Z',
-    subaccount=SUBACCOUNT_API_KEY, # Use to show only the results that contain this key 
-)
-```
-
-### Transfer account balances between accounts
-
-```python
-client.subaccounts.transfer_balance(
-    from_=FROM_ACCOUNT, 
-    to=TO_ACCOUNT, 
-    amount=0.50, 
-    reference='test balance transfer',
-)
-```
-
-### Transfer bought phone numbers between accounts
-
-```python
-client.subaccounts.transfer_balance(
-    from_=FROM_ACCOUNT, 
-    to=TO_ACCOUNT, 
-    number=NUMBER_TO_TRANSFER, 
-    country='US',
-)
-```
-
-## Number Management API
-
-### Get numbers associated with your account
-
-```python
-client.numbers.get_account_numbers(size=25)
-```
-
-### Get numbers that are available to buy
-
-```python
-client.numbers.get_available_numbers('CA', size=25)
-```
-
-### Buy an available number
-
-```python
-params = {'country': 'US', 'msisdn': 'number_to_buy'}
-client.numbers.buy_number(params)
-
-# To buy a number for a subaccount
-params = {'country': 'US', 'msisdn': 'number_to_buy', 'target_api_key': SUBACCOUNT_API_KEY}
-client.numbers.buy_number(params)
-```
-
-### Cancel your subscription for a specific number
-
-```python
-params = {'country': 'US', 'msisdn': 'number_to_cancel'}
-client.numbers.cancel_number(params)
-
-# To cancel a number assigned to a subaccount
-params = {'country': 'US', 'msisdn': 'number_to_buy', 'target_api_key': SUBACCOUNT_API_KEY}
-client.numbers.cancel_number(params)
-```
-
-### Update the behaviour of a number that you own
-
-```python
-params = {"country": "US", "msisdn": "number_to_update", "moHttpUrl": "callback_url"}
-client.numbers.update_number(params)
-```
-
 ## Pricing API
 
 ### Get pricing for a single country
 ```python
 client.account.get_country_pricing(country_code='GB', type='sms') # Default type is sms
 ```
 
@@ -1116,54 +587,56 @@
 Docs: [https://developer.nexmo.com/concepts/guides/signing-messages](https://developer.nexmo.com/concepts/guides/signing-messages?utm_source=DEV_REL&utm_medium=github&utm_campaign=python-client-library)
 
 Note: you'll need to contact support@nexmo.com to enable message signing on
 your account before you can validate webhook signatures.
 
 ## JWT parameters
 
-By default, the library generates 15-minute tokens for JWT authentication.
+By default, the library generates short-lived tokens for JWT authentication.
 
-Use the `auth` method of the client class to specify custom parameters:
+Use the auth method to specify parameters for a longer life token or to
+specify a different token identifier:
 
 ```python
 client.auth(nbf=nbf, exp=exp, jti=jti)
-# OR
-client.auth({'nbf': nbf, 'exp': exp, 'jti': jti})
 ```
 
 ## Overriding API Attributes
 
-In order to rewrite/get the value of variables used across all the Vonage classes Python uses `Call by Object Reference` that allows you to create a single client to use with all API classes.
+In order to rewrite/get the value of variables used across all the Vonage classes Python uses `Call by Object Reference` that allows you to create a single client for Sms/Voice Classes. This means that if you make a change on a client instance this will be available for the Sms class.
 
 An example using setters/getters with `Object references`:
 
 ```python
-from vonage import Client
+from vonage import Client, Sms
 
-# Define the client
+#Defines the client
 client = Client(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
 print(client.host()) # using getter for host -- value returned: rest.nexmo.com
 
-# Change the value in client
-client.host('mio.nexmo.com') # Change host to mio.nexmo.com - this change will be available for sms
-client.sms.send_message(params) # Sends an SMS to the host above
+#Define the sms instance
+sms = Sms(client)
+
+#Change the value in client
+client.host('mio.nexmo.com') #Change host to mio.nexmo.com - this change will be available for sms
+
 ```
 
 ### Overriding API Host / Host Attributes
 
 These attributes are private in the client class and the only way to access them is using the getters/setters we provide.
 
 ```python
 from vonage import Client
 
 client = Client(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
 print(client.host()) # return rest.nexmo.com
-client.host('newhost.vonage.com') # rewrites the host value to newhost.vonage.com
+client.host('mio.nexmo.com') # rewrites the host value to mio.nexmo.com
 print(client.api_host()) # returns api.vonage.com
-client.api_host('myapi.vonage.com') # rewrite the value of api_host to myapi.vonage.com
+client.api_host('myapi.vonage.com') # rewrite the value of api_host
 ```
 
 ## Frequently Asked Questions
 
 ### Supported APIs
 
 The following is a list of Vonage APIs and whether the Python SDK provides support for them:
@@ -1174,27 +647,25 @@
 | Alerts API            | General Availability |     ✅     |
 | Application API       | General Availability |     ✅     |
 | Audit API             |         Beta         |     ❌     |
 | Conversation API      |         Beta         |     ❌     |
 | Dispatch API          |         Beta         |     ❌     |
 | External Accounts API |         Beta         |     ❌     |
 | Media API             |         Beta         |     ❌     |
-| Meetings API          | General Availability |     ✅     |
 | Messages API          | General Availability |     ✅     |
 | Number Insight API    | General Availability |     ✅     |
 | Number Management API | General Availability |     ✅     |
 | Pricing API           | General Availability |     ✅     |
 | Redact API            |   Developer Preview  |     ❌     |
 | Reports API           |         Beta         |     ❌     |
 | SMS API               | General Availability |     ✅     |
-| Subaccounts API       | General Availability |     ✅     |
 | Verify API            | General Availability |     ✅     |
 | Voice API             | General Availability |     ✅     |
 
-### asyncio Support
+## asyncio Support
 
 [asyncio](https://docs.python.org/3/library/asyncio.html) is a library to write **concurrent** code using the **async/await** syntax.
 
 We don't currently support asyncio in the Python SDK but we are planning to do so in upcoming releases.
 
 ## Contributing
```

### Comparing `vonage-3.7.1/setup.py` & `vonage-4.0.0b0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import io
 import os
 
 from setuptools import setup, find_packages
 
 
-with io.open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
+with io.open(
+    os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8"
+) as f:
     long_description = f.read()
 
 setup(
     name="vonage",
-    version="3.7.1",
+    version="4.0.0b0",
     description="Vonage Server SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Vonage/vonage-python-sdk",
     author="Vonage",
     author_email="devrel@vonage.com",
     license="Apache",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     platforms=["any"],
     install_requires=[
-        "vonage-jwt>=1.0.0",
         "requests>=2.4.2",
+        "PyJWT[crypto]>=1.6.4",
         "pytz>=2018.5",
         "Deprecated",
-        "pydantic>=1.10,==1.*",
     ],
     python_requires=">=3.7",
     tests_require=["cryptography>=2.3.1"],
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
```

### Comparing `vonage-3.7.1/src/vonage/account.py` & `vonage-4.0.0b0/src/vonage/account.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/src/vonage/application.py` & `vonage-4.0.0b0/src/vonage/application.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/src/vonage/client.py` & `vonage-4.0.0b0/src/vonage/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 import vonage
-from vonage_jwt.jwt import JwtClient
 
 from .account import Account
 from .application import ApplicationV2, Application
 from .errors import *
-from .meetings import Meetings
 from .messages import Messages
 from .number_insight import NumberInsight
-from .number_management import Numbers
-from .proactive_connect import ProactiveConnect
+from .numbers import Numbers
 from .redact import Redact
 from .short_codes import ShortCodes
 from .sms import Sms
-from .subaccounts import Subaccounts
 from .ussd import Ussd
+from .video import Video
 from .voice import Voice
 from .verify import Verify
-from .verify2 import Verify2
 
 import logging
 from platform import python_version
 
 import base64
 import hashlib
 import hmac
+import jwt
 import os
 import time
+import re
+from uuid import uuid4
 
-from requests import Response
 from requests.adapters import HTTPAdapter
 from requests.sessions import Session
 
 string_types = (str, bytes)
 
 try:
     from json import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 
 logger = logging.getLogger("vonage")
 
-
 class Client:
     """
     Create a Client object to start making calls to Vonage/Nexmo APIs.
 
     The credentials you provide when instantiating a Client determine which
     methods can be called. Consult the `Vonage API docs <https://developer.vonage.com/concepts/guides/authentication/>`
     for details of the authentication used by the APIs you wish to use, and instantiate your
@@ -78,104 +75,103 @@
         secret=None,
         signature_secret=None,
         signature_method=None,
         application_id=None,
         private_key=None,
         app_name=None,
         app_version=None,
-        timeout=None,
-        pool_connections=10,
-        pool_maxsize=10,
-        max_retries=3,
+        timeout=None, 
+        pool_connections=10, 
+        pool_maxsize=10, 
+        max_retries=3
     ):
         self.api_key = key or os.environ.get("VONAGE_API_KEY", None)
         self.api_secret = secret or os.environ.get("VONAGE_API_SECRET", None)
 
         self.signature_secret = signature_secret or os.environ.get("VONAGE_SIGNATURE_SECRET", None)
         self.signature_method = signature_method or os.environ.get("VONAGE_SIGNATURE_METHOD", None)
 
         if self.signature_method in {"md5", "sha1", "sha256", "sha512"}:
             self.signature_method = getattr(hashlib, signature_method)
 
+        self._jwt_auth_params = {}
+
         if private_key is not None and application_id is not None:
-            self._jwt_client = JwtClient(application_id, private_key)
+            self.application_id = application_id
+            self._private_key = private_key
+
+            if isinstance(self._private_key, string_types) and re.search("[.][a-zA-Z0-9_]+$", self._private_key):
+                with open(self._private_key, "rb") as key_file:
+                    self._private_key = key_file.read()
 
-        self._jwt_claims = {}
         self._host = "rest.nexmo.com"
         self._api_host = "api.nexmo.com"
-        self._meetings_api_host = "api-eu.vonage.com/beta/meetings"
-        self._proactive_connect_host = "api-eu.vonage.com"
+        self._video_host = "video.api.vonage.com"
 
         user_agent = f"vonage-python/{vonage.__version__} python/{python_version()}"
 
         if app_name and app_version:
             user_agent += f" {app_name}/{app_version}"
 
         self.headers = {"User-Agent": user_agent, "Accept": "application/json"}
 
         self.account = Account(self)
         self.application = Application(self)
-        self.meetings = Meetings(self)
         self.messages = Messages(self)
         self.number_insight = NumberInsight(self)
         self.numbers = Numbers(self)
-        self.proactive_connect = ProactiveConnect(self)
         self.short_codes = ShortCodes(self)
         self.sms = Sms(self)
-        self.subaccounts = Subaccounts(self)
         self.ussd = Ussd(self)
+        self.video = Video(self)
         self.verify = Verify(self)
-        self.verify2 = Verify2(self)
         self.voice = Voice(self)
 
         self.timeout = timeout
         self.session = Session()
         self.adapter = HTTPAdapter(
-            pool_connections=pool_connections, pool_maxsize=pool_maxsize, max_retries=max_retries
+            pool_connections=pool_connections, 
+            pool_maxsize=pool_maxsize, 
+            max_retries=max_retries
         )
         self.session.mount("https://", self.adapter)
 
-    # Gets and sets _host attribute
+    # Get and Set _host attribute
     def host(self, value=None):
         if value is None:
             return self._host
         else:
             self._host = value
 
-    # Gets and sets _api_host attribute
+    # Gets And Set _api_host attribute
     def api_host(self, value=None):
         if value is None:
             return self._api_host
         else:
             self._api_host = value
 
-    # Gets and sets _meetings_api_host attribute
-    def meetings_api_host(self, value=None):
-        if value is None:
-            return self._meetings_api_host
-        else:
-            self._meetings_api_host = value
-
-    def proactive_connect_host(self, value=None):
+    def video_host(self, value=None):
         if value is None:
-            return self._proactive_connect_host
+            return self._video_host
         else:
-            self._proactive_connect_host = value
+            self._video_host = value
 
     def auth(self, params=None, **kwargs):
-        self._jwt_claims = params or kwargs
+        self._jwt_auth_params = params or kwargs
 
     def check_signature(self, params):
         params = dict(params)
         signature = params.pop("sig", "").lower()
         return hmac.compare_digest(signature, self.signature(params))
 
     def signature(self, params):
         if self.signature_method:
-            hasher = hmac.new(self.signature_secret.encode(), digestmod=self.signature_method)
+            hasher = hmac.new(
+                self.signature_secret.encode(), digestmod=self.signature_method
+            )
         else:
             hasher = hashlib.md5()
 
         # Add timestamp if not already present
         if not params.get("timestamp"):
             params["timestamp"] = int(time.time())
 
@@ -193,213 +189,185 @@
         return hasher.hexdigest()
 
     def get(self, host, request_uri, params=None, auth_type=None):
         uri = f"https://{host}{request_uri}"
         self._request_headers = self.headers
 
         if auth_type == 'jwt':
-            self._request_headers['Authorization'] = self._create_jwt_auth_string()
+            self._request_headers = self._add_jwt_to_request_headers()
         elif auth_type == 'params':
-            params = dict(params or {}, api_key=self.api_key, api_secret=self.api_secret)
+            params = dict(
+                params or {}, api_key=self.api_key, api_secret=self.api_secret
+            )
         elif auth_type == 'header':
-            self._request_headers['Authorization'] = self._create_header_auth_string()
+            hash = base64.b64encode(
+                f"{self.api_key}:{self.api_secret}".encode("utf-8")
+            ).decode("ascii")
+            self._request_headers = dict(self.headers or {}, Authorization=f"Basic {hash}")
         else:
             raise InvalidAuthenticationTypeError(
                 f'Invalid authentication type. Must be one of "jwt", "header" or "params".'
             )
 
-        logger.debug(
-            f"GET to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}"
-        )
+        logger.debug(f"GET to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}")
         return self.parse(
-            host,
-            self.session.get(
-                uri, params=params, headers=self._request_headers, timeout=self.timeout
-            ),
-        )
+            host, 
+            self.session.get(uri, params=params, headers=self._request_headers, timeout=self.timeout))
 
-    def post(
-        self,
-        host,
-        request_uri,
-        params,
-        auth_type=None,
-        body_is_json=True,
-        supports_signature_auth=False,
-    ):
+    def post(self, host, request_uri, params, auth_type=None, body_is_json=True, supports_signature_auth=False):
         """
         Low-level method to make a post request to an API server.
         This method automatically adds authentication, picking the first applicable authentication method from the following:
-        - If the supports_signature_auth param is True, and the client was instantiated with a signature_secret,
+        - If the supports_signature_auth param is True, and the client was instantiated with a signature_secret, 
             then signature authentication will be used.
-        :param bool supports_signature_auth: Preferentially use signature authentication if a signature_secret was provided
+        :param bool supports_signature_auth: Preferentially use signature authentication if a signature_secret was provided 
             when initializing this client.
         """
         uri = f"https://{host}{request_uri}"
         self._request_headers = self.headers
-
+        
         if supports_signature_auth and self.signature_secret:
             params["api_key"] = self.api_key
             params["sig"] = self.signature(params)
         elif auth_type == 'jwt':
-            self._request_headers['Authorization'] = self._create_jwt_auth_string()
+            self._request_headers = self._add_jwt_to_request_headers()
         elif auth_type == 'params':
-            params = dict(params, api_key=self.api_key, api_secret=self.api_secret)
+            params = dict(
+                params, api_key=self.api_key, api_secret=self.api_secret
+            )
         elif auth_type == 'header':
-            self._request_headers['Authorization'] = self._create_header_auth_string()
+            hash = base64.b64encode(
+                f"{self.api_key}:{self.api_secret}".encode("utf-8")
+            ).decode("ascii")
+            self._request_headers = dict(self.headers or {}, Authorization=f"Basic {hash}")
         else:
             raise InvalidAuthenticationTypeError(
                 f'Invalid authentication type. Must be one of "jwt", "header" or "params".'
             )
-
-        logger.debug(
-            f"POST to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}"
-        )
+        
+        logger.debug(f"POST to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}")
         if body_is_json:
             return self.parse(
-                host,
-                self.session.post(
-                    uri, json=params, headers=self._request_headers, timeout=self.timeout
-                ),
-            )
+                host, self.session.post(uri, json=params, headers=self._request_headers, timeout=self.timeout))
         else:
             return self.parse(
-                host,
-                self.session.post(
-                    uri, data=params, headers=self._request_headers, timeout=self.timeout
-                ),
-            )
+                host, self.session.post(uri, data=params, headers=self._request_headers, timeout=self.timeout))
 
     def put(self, host, request_uri, params, auth_type=None):
         uri = f"https://{host}{request_uri}"
         self._request_headers = self.headers
 
         if auth_type == 'jwt':
-            self._request_headers['Authorization'] = self._create_jwt_auth_string()
+            self._request_headers = self._add_jwt_to_request_headers()
         elif auth_type == 'header':
-            self._request_headers['Authorization'] = self._create_header_auth_string()
+            hash = base64.b64encode(
+                f"{self.api_key}:{self.api_secret}".encode("utf-8")
+            ).decode("ascii")
+            self._request_headers = dict(self._request_headers or {}, Authorization=f"Basic {hash}")
         else:
             raise InvalidAuthenticationTypeError(
-                f'Invalid authentication type. Must be one of "jwt", "header" or "params".'
+                f'Invalid authentication type. Must be one of "jwt" or "header".'
             )
 
-        logger.debug(
-            f"PUT to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}"
-        )
+        logger.debug(f"PUT to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}")
         # All APIs that currently use put methods require a json-formatted body so don't need to check this
-        return self.parse(
-            host,
-            self.session.put(uri, json=params, headers=self._request_headers, timeout=self.timeout),
-        )
+        return self.parse(host, self.session.put(uri, json=params, headers=self._request_headers, timeout=self.timeout))
 
-    def patch(self, host, request_uri, params, auth_type=None):
+    def patch(self, host, request_uri, params, auth_type='jwt'):
         uri = f"https://{host}{request_uri}"
         self._request_headers = self.headers
 
         if auth_type == 'jwt':
-            self._request_headers['Authorization'] = self._create_jwt_auth_string()
-        elif auth_type == 'header':
-            self._request_headers['Authorization'] = self._create_header_auth_string()
+            self._request_headers = self._add_jwt_to_request_headers()
         else:
-            raise InvalidAuthenticationTypeError(f"""Invalid authentication type.""")
+            raise InvalidAuthenticationTypeError(
+                f"""Invalid authentication type. Must be "jwt", as only the Video API 
+                    (which uses jwt auth) currently uses this method."""
+            )
 
-        logger.debug(
-            f"PATCH to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}"
-        )
-        # Only newer APIs (that expect json-bodies) currently use this method, so we will always send a json-formatted body
+        logger.debug(f"PATCH to {repr(uri)} with params {repr(params)}, headers {repr(self._request_headers)}")
+        # Only the Video API currently uses this method, so we will always send a json-formatted body
         return self.parse(host, self.session.patch(uri, json=params, headers=self._request_headers))
 
-    def delete(self, host, request_uri, params=None, auth_type=None):
+    def delete(self, host, request_uri, auth_type=None):
         uri = f"https://{host}{request_uri}"
         self._request_headers = self.headers
 
         if auth_type == 'jwt':
-            self._request_headers['Authorization'] = self._create_jwt_auth_string()
-        elif auth_type == 'header':
-            self._request_headers['Authorization'] = self._create_header_auth_string()
+            self._request_headers = self._add_jwt_to_request_headers()
+        elif auth_type =='header':
+            hash = base64.b64encode(
+                f"{self.api_key}:{self.api_secret}".encode("utf-8")
+            ).decode("ascii")
+            self._request_headers = dict(self._request_headers or {}, Authorization=f"Basic {hash}")
         else:
             raise InvalidAuthenticationTypeError(
                 f'Invalid authentication type. Must be one of "jwt", "header" or "params".'
             )
 
         logger.debug(f"DELETE to {repr(uri)} with headers {repr(self._request_headers)}")
-        if params is not None:
-            logger.debug(f"DELETE call has params {repr(params)}")
         return self.parse(
-            host,
-            self.session.delete(
-                uri, headers=self._request_headers, timeout=self.timeout, params=params
-            ),
+            host, self.session.delete(uri, headers=self._request_headers, timeout=self.timeout)
         )
 
-    def parse(self, host, response: Response):
+    def parse(self, host, response):
         logger.debug(f"Response headers {repr(response.headers)}")
         if response.status_code == 401:
-            raise AuthenticationError("Authentication failed.")
+            raise AuthenticationError(
+                "Authentication failed. Check you're using a valid authentication method."
+            )
         elif response.status_code == 204:
             return None
         elif 200 <= response.status_code < 300:
+
             # Strip off any encoding from the content-type header:
-            try:
-                content_mime = response.headers.get("content-type").split(";", 1)[0]
-            except AttributeError:
-                if response.json() is None:
-                    return None
+            content_mime = response.headers.get("content-type").split(";", 1)[0]
             if content_mime == "application/json":
-                try:
-                    return response.json()
-                except JSONDecodeError:
-                    pass
+                return response.json()
             else:
                 return response.content
         elif 400 <= response.status_code < 500:
-            logger.warning(f"Client error: {response.status_code} {repr(response.content)}")
+            logger.warning(
+                f"Client error: {response.status_code} {repr(response.content)}"
+            )
             message = f"{response.status_code} response from {host}"
 
             # Test for standard error format:
             try:
                 error_data = response.json()
-                if "type" in error_data and "title" in error_data and "detail" in error_data:
-                    title = error_data["title"]
-                    detail = error_data["detail"]
-                    type = error_data["type"]
-                    message = f"{title}: {detail} ({type}){self._add_individual_errors(error_data)}"
-                elif 'status' in error_data and 'message' in error_data and 'name' in error_data:
-                    message = (
-                        f'Status Code {error_data["status"]}: {error_data["name"]}: {error_data["message"]}'
-                        f'{self._add_individual_errors(error_data)}'
-                    )
-                else:
-                    message = error_data
+                if (
+                    "type" in error_data
+                    and "title" in error_data
+                    and "detail" in error_data
+                ):
+                    title=error_data["title"]
+                    detail=error_data["detail"]
+                    type=error_data["type"]
+                    message = f"{title}: {detail} ({type})"
+
             except JSONDecodeError:
                 pass
             raise ClientError(message)
-
         elif 500 <= response.status_code < 600:
             logger.warning(f"Server error: {response.status_code} {repr(response.content)}")
             message = f"{response.status_code} response from {host}"
             raise ServerError(message)
 
-    def _add_individual_errors(self, error_data):
-        message = ''
-        if 'errors' in error_data:
-            for error in error_data["errors"]:
-                message += f"\nError: {error}"
-        return message
-
-    def _create_jwt_auth_string(self):
-        return b"Bearer " + self._generate_application_jwt()
+    def _add_jwt_to_request_headers(self):
+        return dict(self.headers, Authorization=b"Bearer " + self._generate_application_jwt())
 
     def _generate_application_jwt(self):
-        try:
-            return self._jwt_client.generate_application_jwt(self._jwt_claims)
-        except AttributeError as err:
-            if '_jwt_client' in str(err):
-                raise ClientError(
-                    'JWT generation failed. Check that you passed in valid values for "application_id" and "private_key".'
-                )
-            else:
-                raise err
+        iat = int(time.time())
+
+        payload = dict(self._jwt_auth_params)
+        payload.setdefault("application_id", self.application_id)
+        payload.setdefault("iat", iat)
+        payload.setdefault("exp", iat + 60)
+        payload.setdefault("jti", str(uuid4()))
+
+        token = jwt.encode(payload, self._private_key, algorithm="RS256")
+
+        # If token is string transform it to byte type
+        if(type(token) is str):
+            token = bytes(token, 'utf-8')
 
-    def _create_header_auth_string(self):
-        hash = base64.b64encode(f"{self.api_key}:{self.api_secret}".encode("utf-8")).decode("ascii")
-        return f"Basic {hash}"
+        return token
```

### Comparing `vonage-3.7.1/src/vonage/errors.py` & `vonage-4.0.0b0/src/vonage/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,28 +25,22 @@
 
 
 class PricingTypeError(Error):
     """A pricing type was specified that is not allowed."""
 
 
 class RedactError(Error):
-    """Error related to the Redact class or Redact API."""
 
+    """Error related to the Redact class or Redact API."""
 
 class InvalidAuthenticationTypeError(Error):
-    """An authentication method was specified that is not allowed"""
-
-
-class MeetingsError(ClientError):
-    """An error related to the Meetings class which calls the Vonage Meetings API."""
-
-
-class Verify2Error(ClientError):
-    """An error relating to the Verify (V2) API."""
+    """An authentication method was specified that is not allowed."""
 
 
-class SubaccountsError(ClientError):
-    """An error relating to the Subaccounts API."""
+class InvalidRoleError(Error):
+    """The specified role was invalid."""
 
+class TokenExpiryError(Error):
+    """The specified token expiry time was invalid."""
 
-class ProactiveConnectError(ClientError):
-    """An error relating to the Proactive Connect API."""
+class InvalidOptionsError(Error):
+    """The option(s) that were specified are invalid."""
```

### Comparing `vonage-3.7.1/src/vonage/messages.py` & `vonage-4.0.0b0/src/vonage/messages.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,113 +1,84 @@
-from ._internal import set_auth_type
 from .errors import MessagesError
 
 import re
 
-
 class Messages:
     valid_message_channels = {'sms', 'mms', 'whatsapp', 'messenger', 'viber_service'}
     valid_message_types = {
         'sms': {'text'},
         'mms': {'image', 'vcard', 'audio', 'video'},
-        'whatsapp': {'text', 'image', 'audio', 'video', 'file', 'template', 'sticker', 'custom'},
+        'whatsapp': {'text', 'image', 'audio', 'video', 'file', 'template', 'custom'},
         'messenger': {'text', 'image', 'audio', 'video', 'file'},
-        'viber_service': {'text', 'image', 'video', 'file'},
+        'viber_service': {'text', 'image'}
     }
-
+    
     def __init__(self, client):
         self._client = client
-        self._auth_type = set_auth_type(self._client)
+        self._auth_type = 'jwt'
 
-    def send_message(self, params: dict):
+    def send_message(self, params: dict):       
         self.validate_send_message_input(params)
-
+        
+        if not hasattr(self._client, '_application_id'):
+            self._auth_type='header'
         return self._client.post(
-            self._client.api_host(),
+            self._client.api_host(), 
             "/v1/messages",
-            params,
+            params, 
             auth_type=self._auth_type,
-        )
+            )
 
     def validate_send_message_input(self, params):
         self._check_input_is_dict(params)
         self._check_valid_message_channel(params)
         self._check_valid_message_type(params)
         self._check_valid_recipient(params)
         self._check_valid_sender(params)
         self._channel_specific_checks(params)
         self._check_valid_client_ref(params)
-
+    
     def _check_input_is_dict(self, params):
         if type(params) is not dict:
-            raise MessagesError(
-                'Parameters to the send_message method must be specified as a dictionary.'
-            )
+            raise MessagesError('Parameters to the send_message method must be specified as a dictionary.')
 
     def _check_valid_message_channel(self, params):
         if params['channel'] not in Messages.valid_message_channels:
-            raise MessagesError(
-                f"""
-            "{params['channel']}" is an invalid message channel. 
+            raise MessagesError(f"""
+            '{params['channel']}' is an invalid message channel. 
             Must be one of the following types: {self.valid_message_channels}'
-            """
-            )
+            """)
 
     def _check_valid_message_type(self, params):
         if params['message_type'] not in self.valid_message_types[params['channel']]:
-            raise MessagesError(
-                f"""
+            raise MessagesError(f"""
                 "{params['message_type']}" is not a valid message type for channel "{params["channel"]}". 
                 Must be one of the following types: {self.valid_message_types[params["channel"]]}
-            """
-            )
+            """)
 
     def _check_valid_recipient(self, params):
         if not isinstance(params['to'], str):
             raise MessagesError(f'Message recipient ("to={params["to"]}") not in a valid format.')
         elif params['channel'] != 'messenger' and not re.search(r'^[1-9]\d{6,14}$', params['to']):
-            raise MessagesError(
-                f'Message recipient number ("to={params["to"]}") not in a valid format.'
-            )
+            raise MessagesError(f'Message recipient number ("to={params["to"]}") not in a valid format.')
         elif params['channel'] == 'messenger' and not 0 < len(params['to']) < 50:
-            raise MessagesError(
-                f'Message recipient ID ("to={params["to"]}") not in a valid format.'
-            )
+            raise MessagesError(f'Message recipient ID ("to={params["to"]}") not in a valid format.')
 
     def _check_valid_sender(self, params):
         if not isinstance(params['from'], str) or params['from'] == "":
-            raise MessagesError(
-                f'Message sender ("frm={params["from"]}") set incorrectly. Set a valid name or number for the sender.'
-            )
+            raise MessagesError(f'Message sender ("frm={params["from"]}") set incorrectly. Set a valid name or number for the sender.')
 
     def _channel_specific_checks(self, params):
-        if (
-            (
-                params['channel'] == 'whatsapp'
-                and params['message_type'] == 'template'
-                and 'whatsapp' not in params
-            )
-            or (
-                params['channel'] == 'whatsapp'
-                and params['message_type'] == 'sticker'
-                and 'sticker' not in params
-            )
-            or (params['channel'] == 'viber_service' and 'viber_service' not in params)
-        ):
-            raise MessagesError(
-                f'''You must specify all required properties for message channel "{params["channel"]}".'''
-            )
-        elif params['channel'] == 'whatsapp' and params['message_type'] == 'sticker':
-            self._check_valid_whatsapp_sticker(params['sticker'])
+        try:        
+            if params['channel'] == 'whatsapp' and params['message_type'] == 'template':
+                params['whatsapp']
+            if params['channel'] == 'viber_service':
+                params['viber_service']
+        except (KeyError, TypeError):
+            raise MessagesError(f'''You must specify all required properties for message channel "{params["channel"]}".''')
 
     def _check_valid_client_ref(self, params):
         if 'client_ref' in params:
-            if len(params['client_ref']) <= 100:
+            if len(params['client_ref']) <= 40:
                 self._client_ref = params['client_ref']
             else:
-                raise MessagesError('client_ref can be a maximum of 100 characters.')
-
-    def _check_valid_whatsapp_sticker(self, sticker):
-        if ('id' not in sticker and 'url' not in sticker) or ('id' in sticker and 'url' in sticker):
-            raise MessagesError(
-                'Must specify one, and only one, of "id" or "url" in the "sticker" field.'
-            )
+                raise MessagesError('client_ref can be a maximum of 40 characters.')
```

### Comparing `vonage-3.7.1/src/vonage/number_insight.py` & `vonage-4.0.0b0/src/vonage/number_insight.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/src/vonage/number_management.py` & `vonage-4.0.0b0/src/vonage/numbers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 class Numbers:
-    auth_type = 'header'
+    auth_type = 'params'
     defaults = {'auth_type': auth_type, 'body_is_json': False}
 
     def __init__(self, client):
         self._client = client
-
+        
     def get_account_numbers(self, params=None, **kwargs):
         return self._client.get(self._client.host(), "/account/numbers", params or kwargs, auth_type=Numbers.auth_type)
 
     def get_available_numbers(self, country_code, params=None, **kwargs):
         return self._client.get(
-            self._client.host(),
-            "/number/search",
-            dict(params or kwargs, country=country_code),
-            auth_type=Numbers.auth_type,
+            self._client.host(), 
+            "/number/search", 
+            dict(params or kwargs, country=country_code), 
+            auth_type=Numbers.auth_type
         )
 
     def buy_number(self, params=None, **kwargs):
-        return self._client.post(self._client.host(), "/number/buy", params or kwargs, **Numbers.defaults)
+        return self._client.post(
+            self._client.host(), "/number/buy", params or kwargs, **Numbers.defaults
+        )
 
     def cancel_number(self, params=None, **kwargs):
-        return self._client.post(self._client.host(), "/number/cancel", params or kwargs, **Numbers.defaults)
+        return self._client.post(
+            self._client.host(), "/number/cancel", params or kwargs, **Numbers.defaults
+        )
 
     def update_number(self, params=None, **kwargs):
-        return self._client.post(self._client.host(), "/number/update", params or kwargs, **Numbers.defaults)
+        return self._client.post(
+            self._client.host(), "/number/update", params or kwargs, **Numbers.defaults
+        )
```

### Comparing `vonage-3.7.1/src/vonage/redact.py` & `vonage-4.0.0b0/src/vonage/redact.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/src/vonage/short_codes.py` & `vonage-4.0.0b0/src/vonage/short_codes.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/src/vonage/sms.py` & `vonage-4.0.0b0/src/vonage/sms.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/src/vonage/verify.py` & `vonage-4.0.0b0/src/vonage/verify.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
     defaults = {'auth_type': auth_type, 'body_is_json': False}
 
     def __init__(self, client):
         self._client = client
 
     def start_verification(self, params=None, **kwargs):
         return self._client.post(
-            self._client.api_host(),
-            "/verify/json",
+            self._client.api_host(), 
+            "/verify/json", 
             params or kwargs,
             **Verify.defaults,
         )
 
     def check(self, request_id, params=None, **kwargs):
         return self._client.post(
             self._client.api_host(),
@@ -40,12 +40,10 @@
             "/verify/control/json",
             {"request_id": request_id, "cmd": "trigger_next_event"},
             **Verify.defaults,
         )
 
     def psd2(self, params=None, **kwargs):
         return self._client.post(
-            self._client.api_host(),
-            "/verify/psd2/json",
-            params or kwargs,
-            **Verify.defaults,
+            self._client.api_host(), "/verify/psd2/json", params or kwargs, **Verify.defaults,
         )
+
```

### Comparing `vonage-3.7.1/src/vonage/voice.py` & `vonage-4.0.0b0/src/vonage/voice.py`

 * *Files 7% similar despite different names*

```diff
@@ -92,10 +92,8 @@
         return self._client.delete(self._client.api_host(),
             f"/v1/calls/{uuid}/talk", 
             auth_type=Voice.auth_type
         )
 
     def get_recording(self, url):
         hostname = urlparse(url).hostname
-        headers = self._client.headers
-        headers['Authorization'] = self._client._create_jwt_auth_string()
-        return self._client.parse(hostname, self._client.session.get(url, headers=headers))
+        return self._client.parse(hostname, self._client.session.get(url, headers=self._client._add_jwt_to_request_headers()))
```

### Comparing `vonage-3.7.1/tests/conftest.py` & `vonage-4.0.0b0/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,92 @@
 import os
 import os.path
 import platform
 
 import pytest
-
+import vonage
 
 # Ensure our client isn't being configured with real values!
 os.environ.clear()
 
 
 def read_file(path):
     with open(os.path.join(os.path.dirname(__file__), path)) as input_file:
         return input_file.read()
 
 
 class DummyData(object):
     def __init__(self):
-        import vonage
-
         self.api_key = "nexmo-api-key"
         self.api_secret = "nexmo-api-secret"
         self.signature_secret = "secret"
         self.application_id = "nexmo-application-id"
         self.private_key = read_file("data/private_key.txt")
         self.public_key = read_file("data/public_key.txt")
         self.user_agent = f"vonage-python/{vonage.__version__} python/{platform.python_version()}"
         self.host = "rest.nexmo.com"
         self.api_host = "api.nexmo.com"
-        self.meetings_api_host = "api-eu.vonage.com/beta/meetings"
 
 
 @pytest.fixture(scope="session")
 def dummy_data():
     return DummyData()
 
 
 @pytest.fixture
 def client(dummy_data):
-    import vonage
-
     return vonage.Client(
         key=dummy_data.api_key,
         secret=dummy_data.api_secret,
         application_id=dummy_data.application_id,
         private_key=dummy_data.private_key,
     )
 
 
 # Represents an instance of the Voice class for testing
 @pytest.fixture
 def voice(client):
-    import vonage
-
     return vonage.Voice(client)
 
 
 # Represents an instance of the Sms class for testing
 @pytest.fixture
 def sms(client):
-    import vonage
-
     return vonage.Sms(client)
 
 
 # Represents an instance of the Verify class for testing
 @pytest.fixture
 def verify(client):
-    import vonage
-
     return vonage.Verify(client)
 
-
 @pytest.fixture
 def number_insight(client):
-    import vonage
-
     return vonage.NumberInsight(client)
 
-
 @pytest.fixture
 def account(client):
-    import vonage
-
     return vonage.Account(client)
 
-
 @pytest.fixture
 def numbers(client):
-    import vonage
-
     return vonage.Numbers(client)
 
-
 @pytest.fixture
 def ussd(client):
-    import vonage
-
     return vonage.Ussd(client)
 
-
 @pytest.fixture
 def short_codes(client):
-    import vonage
-
     return vonage.ShortCodes(client)
 
-
 @pytest.fixture
 def messages(client):
-    import vonage
-
     return vonage.Messages(client)
 
-
 @pytest.fixture
 def redact(client):
-    import vonage
-
     return vonage.Redact(client)
 
-
 @pytest.fixture
 def application_v2(client):
-    import vonage
-
     return vonage.ApplicationV2(client)
-
-
-@pytest.fixture
-def meetings(client):
-    import vonage
-
-    return vonage.Meetings(client)
-
-
-@pytest.fixture
-def proc(client):
-    import vonage
-
-    return vonage.ProactiveConnect(client)
```

### Comparing `vonage-3.7.1/tests/data/applications/list_applications.json` & `vonage-4.0.0b0/tests/data/applications/list_applications.json`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/data/private_key.txt` & `vonage-4.0.0b0/tests/data/private_key.txt`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_account.py` & `vonage-4.0.0b0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_application.py` & `vonage-4.0.0b0/tests/test_application.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_client.py` & `vonage-4.0.0b0/tests/test_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,7 +29,13 @@
 
     client = vonage.Client(application_id="myid", private_key=dummy_data.private_key, timeout=1)
     voice = vonage.Voice(client)
     voice.create_call("123455")
 
     assert len(responses.calls) == 1
     assert responses.calls[0].request.req_kwargs["timeout"] == 1
+
+
+def test_setting_video_api_host(client):
+    assert client._video_host == 'video.api.vonage.com'
+    client.video_host('new.video.url')
+    assert client._video_host == 'new.video.url'
```

### Comparing `vonage-3.7.1/tests/test_number_insight.py` & `vonage-4.0.0b0/tests/test_number_insight.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_number_management.py` & `vonage-4.0.0b0/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_redact.py` & `vonage-4.0.0b0/tests/test_redact.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_rest_calls.py` & `vonage-4.0.0b0/tests/test_rest_calls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from util import *
 from vonage.errors import InvalidAuthenticationTypeError
 
-
 @responses.activate
 def test_get_with_query_params_auth(client, dummy_data):
     stub(responses.GET, "https://api.nexmo.com/v1/applications")
     host = "api.nexmo.com"
     request_uri = "/v1/applications"
     params = {"aaa": "xxx", "bbb": "yyy"}
     response = client.get(host, request_uri, params=params, auth_type='params')
@@ -81,37 +80,34 @@
     assert isinstance(response, dict)
     assert request_user_agent() == dummy_data.user_agent
     assert_basic_auth()
 
 
 @responses.activate
 def test_patch(client, dummy_data):
-    stub(responses.PATCH, "https://api.nexmo.com/v1/applications")
+    stub(responses.PATCH, f"https://api.nexmo.com/v2/project", fixture_path="rest_calls/patch.json")
     host = "api.nexmo.com"
-    request_uri = "/v1/applications"
-    params = {"aaa": "xxx", "bbb": "yyy"}
+    request_uri = "/v2/project"
+    params = {"test_param_1": "test1", "test_param_2": "test2"}
     response = client.patch(host, request_uri, params=params, auth_type='jwt')
+    assert isinstance(response, dict)
+    assert response['patch'] == 'test_case'
+    assert response['successful'] == True
     assert request_headers()['Content-Type'] == 'application/json'
     assert re.search(b'^Bearer ', request_headers()['Authorization']) is not None
-    assert isinstance(response, dict)
     assert request_user_agent() == dummy_data.user_agent
-    assert b"aaa" in request_body()
-    assert b"xxx" in request_body()
-    assert b"bbb" in request_body()
-    assert b"yyy" in request_body()
+    assert b"test_param_1" in request_body()
+    assert b"test1" in request_body()
+    assert b"test_param_2" in request_body()
+    assert b"test2" in request_body()
 
 
 @responses.activate
 def test_patch_no_content(client, dummy_data):
-    stub(
-        responses.PATCH,
-        f"https://api.nexmo.com/v2/project",
-        status_code=204,
-        fixture_path='no_content.json',
-    )
+    stub(responses.PATCH, f"https://api.nexmo.com/v2/project", status_code=204)
     host = "api.nexmo.com"
     request_uri = "/v2/project"
     params = {"test_param_1": "test1", "test_param_2": "test2"}
     client.patch(host, request_uri, params=params, auth_type='jwt')
     assert request_headers()['Content-Type'] == 'application/json'
     assert re.search(b'^Bearer ', request_headers()['Authorization']) is not None
     assert request_user_agent() == dummy_data.user_agent
@@ -123,17 +119,7 @@
 
 def test_patch_invalid_auth_type(client):
     host = "api.nexmo.com"
     request_uri = "/v2/project"
     params = {"test_param_1": "test1", "test_param_2": "test2"}
     with pytest.raises(InvalidAuthenticationTypeError):
         client.patch(host, request_uri, params=params, auth_type='params')
-
-
-@responses.activate
-def test_get_with_jwt_auth(client, dummy_data):
-    stub(responses.GET, "https://api.nexmo.com/v1/calls")
-    host = "api.nexmo.com"
-    request_uri = "/v1/calls"
-    response = client.get(host, request_uri, auth_type='jwt')
-    assert isinstance(response, dict)
-    assert request_user_agent() == dummy_data.user_agent
```

### Comparing `vonage-3.7.1/tests/test_short_codes.py` & `vonage-4.0.0b0/tests/test_short_codes.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_signature.py` & `vonage-4.0.0b0/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_sms.py` & `vonage-4.0.0b0/tests/test_sms.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_ussd.py` & `vonage-4.0.0b0/tests/test_ussd.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_verify.py` & `vonage-4.0.0b0/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `vonage-3.7.1/tests/test_voice.py` & `vonage-4.0.0b0/tests/test_voice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,46 @@
 import os.path
 import time
 
 import jwt
 
 import vonage
-from vonage import Ncco
 from util import *
 
 
 @responses.activate
 def test_create_call(voice, dummy_data):
     stub(responses.POST, "https://api.nexmo.com/v1/calls")
 
     params = {
         "to": [{"type": "phone", "number": "14843331234"}],
         "from": {"type": "phone", "number": "14843335555"},
-        "answer_url": ["https://example.com/answer"],
+        "answer_url": ["https://example.com/answer"]
     }
 
     assert isinstance(voice.create_call(params), dict)
     assert request_user_agent() == dummy_data.user_agent
     assert request_content_type() == "application/json"
 
-
 @responses.activate
 def test_params_with_random_number(voice, dummy_data):
     stub(responses.POST, "https://api.nexmo.com/v1/calls")
 
     params = {
         "to": [{"type": "phone", "number": "14843331234"}],
-        "random_from_number": True,
-        "answer_url": ["https://example.com/answer"],
+        "random_from_number":True,
+        "answer_url": ["https://example.com/answer"]
     }
 
     assert isinstance(voice.create_call(params), dict)
     assert request_user_agent() == dummy_data.user_agent
     assert request_content_type() == "application/json"
 
 
 @responses.activate
-def test_create_call_with_ncco_builder(voice, dummy_data):
-    stub(responses.POST, "https://api.nexmo.com/v1/calls")
-
-    talk = Ncco.Talk(
-        text='Hello from Vonage!', bargeIn=True, loop=3, level=0.5, language='en-GB', style=1, premium=True
-    )
-    ncco = Ncco.build_ncco(talk)
-    voice.create_call(
-        {
-            'to': [{'type': 'phone', 'number': '447449815316'}],
-            'from': {'type': 'phone', 'number': '447418370240'},
-            'ncco': ncco,
-        }
-    )
-    assert (
-        request_body()
-        == b'{"to": [{"type": "phone", "number": "447449815316"}], "from": {"type": "phone", "number": "447418370240"}, "ncco": [{"action": "talk", "text": "Hello from Vonage!", "bargeIn": true, "loop": 3, "level": 0.5, "language": "en-GB", "style": 1, "premium": true}]}'
-    )
-    assert request_user_agent() == dummy_data.user_agent
-    assert request_content_type() == "application/json"
-
-
-@responses.activate
 def test_get_calls(voice, dummy_data):
     stub(responses.GET, "https://api.nexmo.com/v1/calls")
 
     assert isinstance(voice.get_calls(), dict)
     assert request_user_agent() == dummy_data.user_agent
     assert_re(r"\ABearer ", request_authorization())
 
@@ -135,30 +110,29 @@
     assert isinstance(voice.send_dtmf("xx-xx-xx-xx", digits="1234"), dict)
     assert request_user_agent() == dummy_data.user_agent
     assert request_content_type() == "application/json"
     assert request_body() == b'{"digits": "1234"}'
 
 
 @responses.activate
-def test_user_provided_authorization(dummy_data):
+def test_user_provided_authorization(client, dummy_data):
     stub(responses.GET, "https://api.nexmo.com/v1/calls/xx-xx-xx-xx")
 
-    application_id = "different-application-id"
-    client = vonage.Client(application_id=application_id, private_key=dummy_data.private_key)
-
+    application_id = "different-nexmo-application-id"
     nbf = int(time.time())
     exp = nbf + 3600
-    
-    client.auth(nbf=nbf, exp=exp)
-    client.voice.get_call("xx-xx-xx-xx")
+
+    client.auth(application_id=application_id, nbf=nbf, exp=exp)
+    voice = vonage.Voice(client)
+    voice.get_call("xx-xx-xx-xx")
 
     token = request_authorization().split()[1]
 
     token = jwt.decode(token, dummy_data.public_key, algorithms="RS256")
-    print(token)
+
     assert token["application_id"] == application_id
     assert token["nbf"] == nbf
     assert token["exp"] == exp
 
 
 @responses.activate
 def test_authorization_with_private_key_path(dummy_data):
@@ -171,32 +145,39 @@
         secret=dummy_data.api_secret,
         application_id=dummy_data.application_id,
         private_key=private_key,
     )
     voice = vonage.Voice(client)
     voice.get_call("xx-xx-xx-xx")
 
-    token = jwt.decode(request_authorization().split()[1], dummy_data.public_key, algorithms="RS256")
+    token = jwt.decode(
+        request_authorization().split()[1], dummy_data.public_key, algorithms="RS256"
+    )
     assert token["application_id"] == dummy_data.application_id
 
 
 @responses.activate
 def test_authorization_with_private_key_object(voice, dummy_data):
     stub(responses.GET, "https://api.nexmo.com/v1/calls/xx-xx-xx-xx")
 
     voice.get_call("xx-xx-xx-xx")
 
-    token = jwt.decode(request_authorization().split()[1], dummy_data.public_key, algorithms="RS256")
+    token = jwt.decode(
+        request_authorization().split()[1], dummy_data.public_key, algorithms="RS256"
+    )
     assert token["application_id"] == dummy_data.application_id
 
-
 @responses.activate
 def test_get_recording(voice, dummy_data):
     stub_bytes(
-        responses.GET, "https://api.nexmo.com/v1/files/d6e47a2e-3414-11e8-8c2c-2f8b643ed957", body=b'THISISANMP3'
+        responses.GET,
+        "https://api.nexmo.com/v1/files/d6e47a2e-3414-11e8-8c2c-2f8b643ed957",
     )
 
     assert isinstance(
-        voice.get_recording("https://api.nexmo.com/v1/files/d6e47a2e-3414-11e8-8c2c-2f8b643ed957"),
+        voice.get_recording(
+            "https://api.nexmo.com/v1/files/d6e47a2e-3414-11e8-8c2c-2f8b643ed957"
+        ),
         bytes,
     )
     assert request_user_agent() == dummy_data.user_agent
+
```

### Comparing `vonage-3.7.1/tests/util.py` & `vonage-4.0.0b0/tests/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def request_query():
     return urlparse(responses.calls[0].request.url).query
 
 
 def request_params():
-    """Obtain the query params, as a dict."""
+    """ Obtain the query params, as a dict. """
     return parse_qs(request_query())
 
 
 def request_headers():
     return responses.calls[0].request.headers
 
 
@@ -35,29 +35,34 @@
 
 def request_content_type():
     return responses.calls[0].request.headers["Content-Type"]
 
 
 def stub(method, url, fixture_path=None, status_code=200):
     body = load_fixture(fixture_path) if fixture_path else '{"key":"value"}'
-    responses.add(method, url, body=body, status=status_code, content_type="application/json")
+    responses.add(
+        method, url, body=body, status=status_code, content_type="application/json"
+    )
 
 
-def stub_bytes(method, url, body):
-    responses.add(method, url, body, status=200)
+def stub_bytes(method, url):
+    responses.add(method, url, body=b"THISISANMP3", status=200)
 
 
 def assert_re(pattern, string):
     __tracebackhide__ = True
     if not re.search(pattern, string):
         pytest.fail(f"Cannot find pattern {repr(pattern)} in {repr(string)}")
 
 
 def assert_basic_auth():
     params = request_params()
     assert "api_key" not in params
     assert "api_secret" not in params
-    assert request_headers()["Authorization"] == "Basic bmV4bW8tYXBpLWtleTpuZXhtby1hcGktc2VjcmV0"
+    assert (
+        request_headers()["Authorization"]
+        == "Basic bmV4bW8tYXBpLWtleTpuZXhtby1hcGktc2VjcmV0"
+    )
 
 
 def load_fixture(fixture_path):
     return open(os.path.join(os.path.dirname(__file__), "data", fixture_path)).read()
```

