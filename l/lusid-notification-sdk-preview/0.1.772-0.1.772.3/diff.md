# Comparing `tmp/lusid-notification-sdk-preview-0.1.772.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.772.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.772.tar", last modified: Thu Jul  6 09:39:57 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.772.3.tar", last modified: Wed Jul  5 08:24:23 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.772.tar` & `lusid-notification-sdk-preview-0.1.772.3.tar`

### file list

```diff
@@ -1,64 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7868 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4184 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27783 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     2896 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11055 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10618 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12413 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15029 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     4726 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6879 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    33426 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8104 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8447 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11551 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15899 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2559 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 09:39:57.000000 lusid-notification-sdk-preview-0.1.772/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-06 09:39:26.000000 lusid-notification-sdk-preview-0.1.772/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8392 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52809 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47815 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27787 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16637 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3608 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     9335 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/api_request_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    10620 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15031 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/email_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9780 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9541 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16039 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    35623 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     4112 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8106 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/sms_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    16642 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8449 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11553 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15901 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13100 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/webhook_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:24:23.000000 lusid-notification-sdk-preview-0.1.772.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-05 08:23:56.000000 lusid-notification-sdk-preview-0.1.772.3/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.772/README.md` & `lusid-notification-sdk-preview-0.1.772.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.772
-- Package version: 0.1.772
+- API version: 0.1.772.3
+- Package version: 0.1.772.3
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -109,17 +109,21 @@
 
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
+ - [AmazonSqsNotificationTypeResponse](docs/AmazonSqsNotificationTypeResponse.md)
+ - [ApiRequestNotificationType](docs/ApiRequestNotificationType.md)
+ - [ApiRequestNotificationTypeResponse](docs/ApiRequestNotificationTypeResponse.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
+ - [EmailNotificationTypeResponse](docs/EmailNotificationTypeResponse.md)
  - [EventFieldDefinition](docs/EventFieldDefinition.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
@@ -127,24 +131,27 @@
  - [ManualEventBody](docs/ManualEventBody.md)
  - [ManualEventHeader](docs/ManualEventHeader.md)
  - [ManualEventRequest](docs/ManualEventRequest.md)
  - [MatchingPattern](docs/MatchingPattern.md)
  - [Notification](docs/Notification.md)
  - [NotificationStatus](docs/NotificationStatus.md)
  - [NotificationType](docs/NotificationType.md)
+ - [NotificationTypeResponse](docs/NotificationTypeResponse.md)
  - [ResourceId](docs/ResourceId.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [ResourceListOfEventTypeSchema](docs/ResourceListOfEventTypeSchema.md)
  - [ResourceListOfNotification](docs/ResourceListOfNotification.md)
  - [ResourceListOfSubscription](docs/ResourceListOfSubscription.md)
  - [SmsNotificationType](docs/SmsNotificationType.md)
+ - [SmsNotificationTypeResponse](docs/SmsNotificationTypeResponse.md)
  - [Subscription](docs/Subscription.md)
  - [UpdateNotificationRequest](docs/UpdateNotificationRequest.md)
  - [UpdateSubscription](docs/UpdateSubscription.md)
  - [WebhookNotificationType](docs/WebhookNotificationType.md)
+ - [WebhookNotificationTypeResponse](docs/WebhookNotificationTypeResponse.md)
 
 
 <a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
 Authentication schemes defined for the API:
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/manual_event_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.3'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.772/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.772.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.772\n"\
-               "SDK Package Version: 0.1.772".\
+               "Version of the API: 0.1.772.3\n"\
+               "SDK Package Version: 0.1.772.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/event_field_definition.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/event_field_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/manual_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,15 +38,15 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'notification_id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'notification_type': 'object',
+        'notification_type': 'NotificationTypeResponse',
         'created_at': 'datetime',
         'user_id_created': 'str',
         'modified_at': 'datetime',
         'user_id_modified': 'str',
         'href': 'str'
     }
 
@@ -79,16 +79,16 @@
         
         :param notification_id:  The identifier of the notification (required)
         :type notification_id: str
         :param display_name:  The name of the notification (required)
         :type display_name: str
         :param description:  The summary of the services provided by the notification
         :type description: str
-        :param notification_type:  The type and contents of the notification (required)
-        :type notification_type: object
+        :param notification_type:  (required)
+        :type notification_type: lusid_notification.NotificationTypeResponse
         :param created_at:  The time at which the subscription was made (required)
         :type created_at: datetime
         :param user_id_created:  The user who made the subscription (required)
         :type user_id_created: str
         :param modified_at:  The time at which the subscription was last modified (required)
         :type modified_at: datetime
         :param user_id_modified:  The user who last modified the subscription (required)
@@ -216,30 +216,30 @@
 
         self._description = description
 
     @property
     def notification_type(self):
         """Gets the notification_type of this Notification.  # noqa: E501
 
-        The type and contents of the notification  # noqa: E501
 
         :return: The notification_type of this Notification.  # noqa: E501
-        :rtype: object
+        :rtype: lusid_notification.NotificationTypeResponse
         """
         return self._notification_type
 
     @notification_type.setter
     def notification_type(self, notification_type):
         """Sets the notification_type of this Notification.
 
-        The type and contents of the notification  # noqa: E501
 
         :param notification_type: The notification_type of this Notification.  # noqa: E501
-        :type notification_type: object
+        :type notification_type: lusid_notification.NotificationTypeResponse
         """
+        if self.local_vars_configuration.client_side_validation and notification_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `notification_type`, must not be `None`")  # noqa: E501
 
         self._notification_type = notification_type
 
     @property
     def created_at(self):
         """Gets the created_at of this Notification.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/notification_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -40,154 +40,161 @@
     """
     openapi_types = {
         'type': 'str',
         'api_key_ref': 'str',
         'api_secret_ref': 'str',
         'body': 'str',
         'queue_url_ref': 'str',
+        'http_method': 'str',
+        'path_and_query': 'str',
+        'content': 'object',
         'subject': 'str',
         'plain_text_body': 'str',
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]',
         'recipients': 'list[str]',
-        'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
         'authentication_configuration_item_paths': 'dict[str, str]',
-        'content_type': 'str',
-        'content': 'object'
+        'content_type': 'str'
     }
 
     attribute_map = {
         'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
         'body': 'body',
         'queue_url_ref': 'queueUrlRef',
+        'http_method': 'httpMethod',
+        'path_and_query': 'pathAndQuery',
+        'content': 'content',
         'subject': 'subject',
         'plain_text_body': 'plainTextBody',
         'html_body': 'htmlBody',
         'email_address_to': 'emailAddressTo',
         'email_address_cc': 'emailAddressCc',
         'email_address_bcc': 'emailAddressBcc',
         'recipients': 'recipients',
-        'http_method': 'httpMethod',
         'url': 'url',
         'authentication_type': 'authenticationType',
         'authentication_configuration_item_paths': 'authenticationConfigurationItemPaths',
-        'content_type': 'contentType',
-        'content': 'content'
+        'content_type': 'contentType'
     }
 
     required_map = {
         'type': 'optional',
         'api_key_ref': 'required',
         'api_secret_ref': 'required',
         'body': 'required',
         'queue_url_ref': 'required',
+        'http_method': 'required',
+        'path_and_query': 'required',
+        'content': 'optional',
         'subject': 'required',
         'plain_text_body': 'required',
         'html_body': 'optional',
         'email_address_to': 'required',
         'email_address_cc': 'optional',
         'email_address_bcc': 'optional',
         'recipients': 'required',
-        'http_method': 'required',
         'url': 'required',
         'authentication_type': 'required',
         'authentication_configuration_item_paths': 'optional',
-        'content_type': 'required',
-        'content': 'optional'
+        'content_type': 'required'
     }
 
-    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, http_method=None, path_and_query=None, content=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, local_vars_configuration=None):  # noqa: E501
         """NotificationType - a model defined in OpenAPI"
         
         :param type:  The type of delivery mechanism for this notification
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
         :param body:  The body of the SMS (required)
         :type body: str
         :param queue_url_ref:  Reference to queue url from Configuration Store (required)
         :type queue_url_ref: str
+        :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
+        :type http_method: str
+        :param path_and_query:  The url to send the request to. (required)
+        :type path_and_query: str
+        :param content:  The content of the request
+        :type content: object
         :param subject:  The subject of the email (required)
         :type subject: str
         :param plain_text_body:  The plain text body of the email (required)
         :type plain_text_body: str
         :param html_body:  The HTML body of the email (if any)
         :type html_body: str
         :param email_address_to:  'To' recipients of the email (required)
         :type email_address_to: list[str]
         :param email_address_cc:  'Cc' recipients of the email
         :type email_address_cc: list[str]
         :param email_address_bcc:  'Bcc' recipients of the email
         :type email_address_bcc: list[str]
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
-        :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
-        :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
-        :param content:  The content of the request
-        :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._api_key_ref = None
         self._api_secret_ref = None
         self._body = None
         self._queue_url_ref = None
+        self._http_method = None
+        self._path_and_query = None
+        self._content = None
         self._subject = None
         self._plain_text_body = None
         self._html_body = None
         self._email_address_to = None
         self._email_address_cc = None
         self._email_address_bcc = None
         self._recipients = None
-        self._http_method = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
-        self._content = None
         self.discriminator = None
 
         self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
+        self.http_method = http_method
+        self.path_and_query = path_and_query
+        self.content = content
         self.subject = subject
         self.plain_text_body = plain_text_body
         self.html_body = html_body
         self.email_address_to = email_address_to
         self.email_address_cc = email_address_cc
         self.email_address_bcc = email_address_bcc
         self.recipients = recipients
-        self.http_method = http_method
         self.url = url
         self.authentication_type = authentication_type
         self.authentication_configuration_item_paths = authentication_configuration_item_paths
         self.content_type = content_type
-        self.content = content
 
     @property
     def type(self):
         """Gets the type of this NotificationType.  # noqa: E501
 
         The type of delivery mechanism for this notification  # noqa: E501
 
@@ -323,14 +330,99 @@
         if (self.local_vars_configuration.client_side_validation and
                 queue_url_ref is not None and len(queue_url_ref) < 1):
             raise ValueError("Invalid value for `queue_url_ref`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._queue_url_ref = queue_url_ref
 
     @property
+    def http_method(self):
+        """Gets the http_method of this NotificationType.  # noqa: E501
+
+        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
+
+        :return: The http_method of this NotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._http_method
+
+    @http_method.setter
+    def http_method(self, http_method):
+        """Sets the http_method of this NotificationType.
+
+        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
+
+        :param http_method: The http_method of this NotificationType.  # noqa: E501
+        :type http_method: str
+        """
+        if self.local_vars_configuration.client_side_validation and http_method is None:  # noqa: E501
+            raise ValueError("Invalid value for `http_method`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                http_method is not None and len(http_method) < 1):
+            raise ValueError("Invalid value for `http_method`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._http_method = http_method
+
+    @property
+    def path_and_query(self):
+        """Gets the path_and_query of this NotificationType.  # noqa: E501
+
+        The url to send the request to.  # noqa: E501
+
+        :return: The path_and_query of this NotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._path_and_query
+
+    @path_and_query.setter
+    def path_and_query(self, path_and_query):
+        """Sets the path_and_query of this NotificationType.
+
+        The url to send the request to.  # noqa: E501
+
+        :param path_and_query: The path_and_query of this NotificationType.  # noqa: E501
+        :type path_and_query: str
+        """
+        if self.local_vars_configuration.client_side_validation and path_and_query is None:  # noqa: E501
+            raise ValueError("Invalid value for `path_and_query`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                path_and_query is not None and len(path_and_query) > 16384):
+            raise ValueError("Invalid value for `path_and_query`, length must be less than or equal to `16384`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                path_and_query is not None and len(path_and_query) < 1):
+            raise ValueError("Invalid value for `path_and_query`, length must be greater than or equal to `1`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                path_and_query is not None and not re.search(r'^([A-Za-z0-9-._~:\/?#[\]@!$&\'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$', path_and_query)):  # noqa: E501
+            raise ValueError(r"Invalid value for `path_and_query`, must be a follow pattern or equal to `/^([A-Za-z0-9-._~:\/?#[\]@!$&'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$/`")  # noqa: E501
+
+        self._path_and_query = path_and_query
+
+    @property
+    def content(self):
+        """Gets the content of this NotificationType.  # noqa: E501
+
+        The content of the request  # noqa: E501
+
+        :return: The content of this NotificationType.  # noqa: E501
+        :rtype: object
+        """
+        return self._content
+
+    @content.setter
+    def content(self, content):
+        """Sets the content of this NotificationType.
+
+        The content of the request  # noqa: E501
+
+        :param content: The content of this NotificationType.  # noqa: E501
+        :type content: object
+        """
+
+        self._content = content
+
+    @property
     def subject(self):
         """Gets the subject of this NotificationType.  # noqa: E501
 
         The subject of the email  # noqa: E501
 
         :return: The subject of this NotificationType.  # noqa: E501
         :rtype: str
@@ -537,42 +629,14 @@
         if (self.local_vars_configuration.client_side_validation and
                 recipients is not None and len(recipients) < 1):
             raise ValueError("Invalid value for `recipients`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._recipients = recipients
 
     @property
-    def http_method(self):
-        """Gets the http_method of this NotificationType.  # noqa: E501
-
-        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
-
-        :return: The http_method of this NotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._http_method
-
-    @http_method.setter
-    def http_method(self, http_method):
-        """Sets the http_method of this NotificationType.
-
-        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
-
-        :param http_method: The http_method of this NotificationType.  # noqa: E501
-        :type http_method: str
-        """
-        if self.local_vars_configuration.client_side_validation and http_method is None:  # noqa: E501
-            raise ValueError("Invalid value for `http_method`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                http_method is not None and len(http_method) < 1):
-            raise ValueError("Invalid value for `http_method`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._http_method = http_method
-
-    @property
     def url(self):
         """Gets the url of this NotificationType.  # noqa: E501
 
         The URL to send the request to  # noqa: E501
 
         :return: The url of this NotificationType.  # noqa: E501
         :rtype: str
@@ -677,37 +741,14 @@
             raise ValueError("Invalid value for `content_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 content_type is not None and len(content_type) < 1):
             raise ValueError("Invalid value for `content_type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._content_type = content_type
 
-    @property
-    def content(self):
-        """Gets the content of this NotificationType.  # noqa: E501
-
-        The content of the request  # noqa: E501
-
-        :return: The content of this NotificationType.  # noqa: E501
-        :rtype: object
-        """
-        return self._content
-
-    @content.setter
-    def content(self, content):
-        """Sets the content of this NotificationType.
-
-        The content of the request  # noqa: E501
-
-        :param content: The content of this NotificationType.  # noqa: E501
-        :type content: object
-        """
-
-        self._content = content
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/sms_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/models/webhook_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772
+    The version of the OpenAPI document: 0.1.772.3
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.772/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.772.3/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,21 @@
 lusid_notification/api/notifications_api.py
 lusid_notification/api/subscriptions_api.py
 lusid_notification/models/__init__.py
 lusid_notification/models/access_controlled_action.py
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
+lusid_notification/models/amazon_sqs_notification_type_response.py
+lusid_notification/models/api_request_notification_type.py
+lusid_notification/models/api_request_notification_type_response.py
 lusid_notification/models/create_notification_request.py
 lusid_notification/models/create_subscription.py
 lusid_notification/models/email_notification_type.py
+lusid_notification/models/email_notification_type_response.py
 lusid_notification/models/event_field_definition.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
 lusid_notification/models/identifier_part_schema.py
 lusid_notification/models/link.py
 lusid_notification/models/lusid_problem_details.py
 lusid_notification/models/lusid_validation_problem_details.py
@@ -32,24 +36,27 @@
 lusid_notification/models/manual_event_body.py
 lusid_notification/models/manual_event_header.py
 lusid_notification/models/manual_event_request.py
 lusid_notification/models/matching_pattern.py
 lusid_notification/models/notification.py
 lusid_notification/models/notification_status.py
 lusid_notification/models/notification_type.py
+lusid_notification/models/notification_type_response.py
 lusid_notification/models/resource_id.py
 lusid_notification/models/resource_list_of_access_controlled_resource.py
 lusid_notification/models/resource_list_of_event_type_schema.py
 lusid_notification/models/resource_list_of_notification.py
 lusid_notification/models/resource_list_of_subscription.py
 lusid_notification/models/sms_notification_type.py
+lusid_notification/models/sms_notification_type_response.py
 lusid_notification/models/subscription.py
 lusid_notification/models/update_notification_request.py
 lusid_notification/models/update_subscription.py
 lusid_notification/models/webhook_notification_type.py
+lusid_notification/models/webhook_notification_type_response.py
 lusid_notification/utilities/__init__.py
 lusid_notification/utilities/config_keys.json
 lusid_notification/utilities/config_keys.py
 lusid_notification_sdk_preview.egg-info/PKG-INFO
 lusid_notification_sdk_preview.egg-info/SOURCES.txt
 lusid_notification_sdk_preview.egg-info/dependency_links.txt
 lusid_notification_sdk_preview.egg-info/requires.txt
```

### Comparing `lusid-notification-sdk-preview-0.1.772/setup.py` & `lusid-notification-sdk-preview-0.1.772.3/setup.py`

 * *Files identical despite different names*

