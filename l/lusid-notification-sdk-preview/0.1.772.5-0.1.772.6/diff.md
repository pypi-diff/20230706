# Comparing `tmp/lusid-notification-sdk-preview-0.1.772.5.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.772.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.772.5.tar", last modified: Thu Jul  6 10:06:16 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.772.6.tar", last modified: Thu Jul  6 10:34:39 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.772.5.tar` & `lusid-notification-sdk-preview-0.1.772.6.tar`

### file list

```diff
@@ -1,71 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/
--rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8392 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4898 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52809 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47815 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27787 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16637 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5101 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3608 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9019 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11057 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     8320 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/amazon_sqs_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     9335 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     7301 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/api_request_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    10620 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15031 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10459 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/email_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/event_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     9780 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8023 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9512 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6427 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9541 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6881 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    16039 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    36155 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)    25118 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     8106 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/sms_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    16642 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8449 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11553 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15901 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13100 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/webhook_notification_type_response.py
--rw-r--r--   0 root         (0) root         (0)    13562 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2995 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:06:16.000000 lusid-notification-sdk-preview-0.1.772.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-07-06 10:05:41.000000 lusid-notification-sdk-preview-0.1.772.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8240 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7824 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52809 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47815 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27787 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16637 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5101 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7256 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9019 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11057 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     8320 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/amazon_sqs_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    10620 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15031 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/email_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9780 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8023 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9512 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9541 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10706 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6881 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7438 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    16039 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    33960 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    24079 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)     6100 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7770 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8106 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/sms_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    16642 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8449 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11553 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15901 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13100 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/webhook_notification_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 10:34:39.000000 lusid-notification-sdk-preview-0.1.772.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-07-06 10:34:04.000000 lusid-notification-sdk-preview-0.1.772.6/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/README.md` & `lusid-notification-sdk-preview-0.1.772.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.772.5
-- Package version: 0.1.772.5
+- API version: 0.1.772.6
+- Package version: 0.1.772.6
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -110,16 +110,14 @@
 ## Documentation For Models
 
  - [AccessControlledAction](docs/AccessControlledAction.md)
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
  - [AmazonSqsNotificationTypeResponse](docs/AmazonSqsNotificationTypeResponse.md)
- - [ApiRequestNotificationType](docs/ApiRequestNotificationType.md)
- - [ApiRequestNotificationTypeResponse](docs/ApiRequestNotificationTypeResponse.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
  - [EmailNotificationTypeResponse](docs/EmailNotificationTypeResponse.md)
  - [EventFieldDefinition](docs/EventFieldDefinition.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.772.5"
+__version__ = "0.1.772.6"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
@@ -34,16 +34,14 @@
 from lusid_notification.exceptions import ApiException
 # import models into sdk package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.amazon_sqs_notification_type_response import AmazonSqsNotificationTypeResponse
-from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
-from lusid_notification.models.api_request_notification_type_response import ApiRequestNotificationTypeResponse
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
 from lusid_notification.models.email_notification_type_response import EmailNotificationTypeResponse
 from lusid_notification.models.event_field_definition import EventFieldDefinition
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/event_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/manual_event_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.772.5'
+        header_params['X-LUSID-SDK-Version'] = '0.1.772.6'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
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
-        self.user_agent = 'OpenAPI-Generator/0.1.772.5/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.772.6/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
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
-               "Version of the API: 0.1.772.5\n"\
-               "SDK Package Version: 0.1.772.5".\
+               "Version of the API: 0.1.772.6\n"\
+               "SDK Package Version: 0.1.772.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from lusid_notification.models.access_controlled_action import AccessControlledAction
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.amazon_sqs_notification_type_response import AmazonSqsNotificationTypeResponse
-from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
-from lusid_notification.models.api_request_notification_type_response import ApiRequestNotificationTypeResponse
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
 from lusid_notification.models.email_notification_type_response import EmailNotificationTypeResponse
 from lusid_notification.models.event_field_definition import EventFieldDefinition
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/amazon_sqs_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/amazon_sqs_notification_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/identifier_part_schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class ApiRequestNotificationType(object):
+class IdentifierPartSchema(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,177 +35,220 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
-        'http_method': 'str',
-        'path_and_query': 'str',
-        'content': 'object'
+        'index': 'int',
+        'name': 'str',
+        'display_name': 'str',
+        'description': 'str',
+        'required': 'bool',
+        'links': 'list[Link]'
     }
 
     attribute_map = {
-        'type': 'type',
-        'http_method': 'httpMethod',
-        'path_and_query': 'pathAndQuery',
-        'content': 'content'
+        'index': 'index',
+        'name': 'name',
+        'display_name': 'displayName',
+        'description': 'description',
+        'required': 'required',
+        'links': 'links'
     }
 
     required_map = {
-        'type': 'required',
-        'http_method': 'required',
-        'path_and_query': 'required',
-        'content': 'optional'
+        'index': 'required',
+        'name': 'required',
+        'display_name': 'required',
+        'description': 'required',
+        'required': 'required',
+        'links': 'optional'
     }
 
-    def __init__(self, type=None, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
-        """ApiRequestNotificationType - a model defined in OpenAPI"
+    def __init__(self, index=None, name=None, display_name=None, description=None, required=None, links=None, local_vars_configuration=None):  # noqa: E501
+        """IdentifierPartSchema - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification (required)
-        :type type: str
-        :param http_method:  The HTTP method such as GET, POST, etc. to use on the Api Request (required)
-        :type http_method: str
-        :param path_and_query:  The url to send the request to. (required)
-        :type path_and_query: str
-        :param content:  The content of the request
-        :type content: object
+        :param index:  (required)
+        :type index: int
+        :param name:  (required)
+        :type name: str
+        :param display_name:  (required)
+        :type display_name: str
+        :param description:  (required)
+        :type description: str
+        :param required:  (required)
+        :type required: bool
+        :param links: 
+        :type links: list[lusid_notification.Link]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
-        self._http_method = None
-        self._path_and_query = None
-        self._content = None
+        self._index = None
+        self._name = None
+        self._display_name = None
+        self._description = None
+        self._required = None
+        self._links = None
         self.discriminator = None
 
-        self.type = type
-        self.http_method = http_method
-        self.path_and_query = path_and_query
-        self.content = content
+        self.index = index
+        self.name = name
+        self.display_name = display_name
+        self.description = description
+        self.required = required
+        self.links = links
 
     @property
-    def type(self):
-        """Gets the type of this ApiRequestNotificationType.  # noqa: E501
+    def index(self):
+        """Gets the index of this IdentifierPartSchema.  # noqa: E501
 
-        The type of delivery mechanism for this notification  # noqa: E501
 
-        :return: The type of this ApiRequestNotificationType.  # noqa: E501
-        :rtype: str
+        :return: The index of this IdentifierPartSchema.  # noqa: E501
+        :rtype: int
         """
-        return self._type
+        return self._index
+
+    @index.setter
+    def index(self, index):
+        """Sets the index of this IdentifierPartSchema.
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ApiRequestNotificationType.
-
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this ApiRequestNotificationType.  # noqa: E501
-        :type type: str
-        """
-        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
-            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        allowed_values = ["ApiRequest"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
-                .format(type, allowed_values)
-            )
 
-        self._type = type
+        :param index: The index of this IdentifierPartSchema.  # noqa: E501
+        :type index: int
+        """
+        if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
+            raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
+
+        self._index = index
 
     @property
-    def http_method(self):
-        """Gets the http_method of this ApiRequestNotificationType.  # noqa: E501
+    def name(self):
+        """Gets the name of this IdentifierPartSchema.  # noqa: E501
 
-        The HTTP method such as GET, POST, etc. to use on the Api Request  # noqa: E501
 
-        :return: The http_method of this ApiRequestNotificationType.  # noqa: E501
+        :return: The name of this IdentifierPartSchema.  # noqa: E501
         :rtype: str
         """
-        return self._http_method
+        return self._name
 
-    @http_method.setter
-    def http_method(self, http_method):
-        """Sets the http_method of this ApiRequestNotificationType.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this IdentifierPartSchema.
 
-        The HTTP method such as GET, POST, etc. to use on the Api Request  # noqa: E501
 
-        :param http_method: The http_method of this ApiRequestNotificationType.  # noqa: E501
-        :type http_method: str
+        :param name: The name of this IdentifierPartSchema.  # noqa: E501
+        :type name: str
         """
-        if self.local_vars_configuration.client_side_validation and http_method is None:  # noqa: E501
-            raise ValueError("Invalid value for `http_method`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                http_method is not None and len(http_method) < 1):
-            raise ValueError("Invalid value for `http_method`, length must be greater than or equal to `1`")  # noqa: E501
+                name is not None and len(name) < 1):
+            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._http_method = http_method
+        self._name = name
 
     @property
-    def path_and_query(self):
-        """Gets the path_and_query of this ApiRequestNotificationType.  # noqa: E501
+    def display_name(self):
+        """Gets the display_name of this IdentifierPartSchema.  # noqa: E501
 
-        The url to send the request to.  # noqa: E501
 
-        :return: The path_and_query of this ApiRequestNotificationType.  # noqa: E501
+        :return: The display_name of this IdentifierPartSchema.  # noqa: E501
         :rtype: str
         """
-        return self._path_and_query
+        return self._display_name
 
-    @path_and_query.setter
-    def path_and_query(self, path_and_query):
-        """Sets the path_and_query of this ApiRequestNotificationType.
+    @display_name.setter
+    def display_name(self, display_name):
+        """Sets the display_name of this IdentifierPartSchema.
 
-        The url to send the request to.  # noqa: E501
 
-        :param path_and_query: The path_and_query of this ApiRequestNotificationType.  # noqa: E501
-        :type path_and_query: str
+        :param display_name: The display_name of this IdentifierPartSchema.  # noqa: E501
+        :type display_name: str
         """
-        if self.local_vars_configuration.client_side_validation and path_and_query is None:  # noqa: E501
-            raise ValueError("Invalid value for `path_and_query`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                path_and_query is not None and len(path_and_query) > 16384):
-            raise ValueError("Invalid value for `path_and_query`, length must be less than or equal to `16384`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                path_and_query is not None and len(path_and_query) < 1):
-            raise ValueError("Invalid value for `path_and_query`, length must be greater than or equal to `1`")  # noqa: E501
+                display_name is not None and len(display_name) < 1):
+            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._display_name = display_name
+
+    @property
+    def description(self):
+        """Gets the description of this IdentifierPartSchema.  # noqa: E501
+
+
+        :return: The description of this IdentifierPartSchema.  # noqa: E501
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this IdentifierPartSchema.
+
+
+        :param description: The description of this IdentifierPartSchema.  # noqa: E501
+        :type description: str
+        """
+        if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
+            raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                path_and_query is not None and not re.search(r'^([A-Za-z0-9-._~:\/?#[\]@!$&\'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$', path_and_query)):  # noqa: E501
-            raise ValueError(r"Invalid value for `path_and_query`, must be a follow pattern or equal to `/^([A-Za-z0-9-._~:\/?#[\]@!$&'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$/`")  # noqa: E501
+                description is not None and len(description) < 1):
+            raise ValueError("Invalid value for `description`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._description = description
+
+    @property
+    def required(self):
+        """Gets the required of this IdentifierPartSchema.  # noqa: E501
+
+
+        :return: The required of this IdentifierPartSchema.  # noqa: E501
+        :rtype: bool
+        """
+        return self._required
+
+    @required.setter
+    def required(self, required):
+        """Sets the required of this IdentifierPartSchema.
+
+
+        :param required: The required of this IdentifierPartSchema.  # noqa: E501
+        :type required: bool
+        """
+        if self.local_vars_configuration.client_side_validation and required is None:  # noqa: E501
+            raise ValueError("Invalid value for `required`, must not be `None`")  # noqa: E501
 
-        self._path_and_query = path_and_query
+        self._required = required
 
     @property
-    def content(self):
-        """Gets the content of this ApiRequestNotificationType.  # noqa: E501
+    def links(self):
+        """Gets the links of this IdentifierPartSchema.  # noqa: E501
 
-        The content of the request  # noqa: E501
 
-        :return: The content of this ApiRequestNotificationType.  # noqa: E501
-        :rtype: object
+        :return: The links of this IdentifierPartSchema.  # noqa: E501
+        :rtype: list[lusid_notification.Link]
         """
-        return self._content
+        return self._links
 
-    @content.setter
-    def content(self, content):
-        """Sets the content of this ApiRequestNotificationType.
+    @links.setter
+    def links(self, links):
+        """Sets the links of this IdentifierPartSchema.
 
-        The content of the request  # noqa: E501
 
-        :param content: The content of this ApiRequestNotificationType.  # noqa: E501
-        :type content: object
+        :param links: The links of this IdentifierPartSchema.  # noqa: E501
+        :type links: list[lusid_notification.Link]
         """
 
-        self._content = content
+        self._links = links
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -241,18 +284,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiRequestNotificationType):
+        if not isinstance(other, IdentifierPartSchema):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiRequestNotificationType):
+        if not isinstance(other, IdentifierPartSchema):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/api_request_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/matching_pattern.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class ApiRequestNotificationTypeResponse(object):
+class MatchingPattern(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,153 +35,113 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'type': 'str',
-        'http_method': 'str',
-        'path_and_query': 'str',
-        'content': 'object'
+        'event_type': 'str',
+        'filter': 'str'
     }
 
     attribute_map = {
-        'type': 'type',
-        'http_method': 'httpMethod',
-        'path_and_query': 'pathAndQuery',
-        'content': 'content'
+        'event_type': 'eventType',
+        'filter': 'filter'
     }
 
     required_map = {
-        'type': 'optional',
-        'http_method': 'optional',
-        'path_and_query': 'optional',
-        'content': 'optional'
+        'event_type': 'required',
+        'filter': 'optional'
     }
 
-    def __init__(self, type=None, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
-        """ApiRequestNotificationTypeResponse - a model defined in OpenAPI"
+    def __init__(self, event_type=None, filter=None, local_vars_configuration=None):  # noqa: E501
+        """MatchingPattern - a model defined in OpenAPI"
         
-        :param type:  The type of delivery mechanism for this notification
-        :type type: str
-        :param http_method:  The HTTP method such as GET, POST, etc. to use on the Api Request
-        :type http_method: str
-        :param path_and_query:  The url to send the request to.
-        :type path_and_query: str
-        :param content:  The content of the request
-        :type content: object
+        :param event_type:  The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint. (required)
+        :type event_type: str
+        :param filter:  A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched
+        :type filter: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._type = None
-        self._http_method = None
-        self._path_and_query = None
-        self._content = None
+        self._event_type = None
+        self._filter = None
         self.discriminator = None
 
-        self.type = type
-        self.http_method = http_method
-        self.path_and_query = path_and_query
-        self.content = content
+        self.event_type = event_type
+        self.filter = filter
 
     @property
-    def type(self):
-        """Gets the type of this ApiRequestNotificationTypeResponse.  # noqa: E501
+    def event_type(self):
+        """Gets the event_type of this MatchingPattern.  # noqa: E501
 
-        The type of delivery mechanism for this notification  # noqa: E501
+        The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint.  # noqa: E501
 
-        :return: The type of this ApiRequestNotificationTypeResponse.  # noqa: E501
+        :return: The event_type of this MatchingPattern.  # noqa: E501
         :rtype: str
         """
-        return self._type
+        return self._event_type
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this ApiRequestNotificationTypeResponse.
+    @event_type.setter
+    def event_type(self, event_type):
+        """Sets the event_type of this MatchingPattern.
+
+        The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint.  # noqa: E501
+
+        :param event_type: The event_type of this MatchingPattern.  # noqa: E501
+        :type event_type: str
+        """
+        if self.local_vars_configuration.client_side_validation and event_type is None:  # noqa: E501
+            raise ValueError("Invalid value for `event_type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                event_type is not None and len(event_type) > 512):
+            raise ValueError("Invalid value for `event_type`, length must be less than or equal to `512`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                event_type is not None and len(event_type) < 0):
+            raise ValueError("Invalid value for `event_type`, length must be greater than or equal to `0`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                event_type is not None and not re.search(r'^[a-zA-Z]*$', event_type)):  # noqa: E501
+            raise ValueError(r"Invalid value for `event_type`, must be a follow pattern or equal to `/^[a-zA-Z]*$/`")  # noqa: E501
 
-        The type of delivery mechanism for this notification  # noqa: E501
-
-        :param type: The type of this ApiRequestNotificationTypeResponse.  # noqa: E501
-        :type type: str
-        """
-
-        self._type = type
-
-    @property
-    def http_method(self):
-        """Gets the http_method of this ApiRequestNotificationTypeResponse.  # noqa: E501
-
-        The HTTP method such as GET, POST, etc. to use on the Api Request  # noqa: E501
-
-        :return: The http_method of this ApiRequestNotificationTypeResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._http_method
-
-    @http_method.setter
-    def http_method(self, http_method):
-        """Sets the http_method of this ApiRequestNotificationTypeResponse.
-
-        The HTTP method such as GET, POST, etc. to use on the Api Request  # noqa: E501
-
-        :param http_method: The http_method of this ApiRequestNotificationTypeResponse.  # noqa: E501
-        :type http_method: str
-        """
-
-        self._http_method = http_method
+        self._event_type = event_type
 
     @property
-    def path_and_query(self):
-        """Gets the path_and_query of this ApiRequestNotificationTypeResponse.  # noqa: E501
+    def filter(self):
+        """Gets the filter of this MatchingPattern.  # noqa: E501
 
-        The url to send the request to.  # noqa: E501
+        A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched  # noqa: E501
 
-        :return: The path_and_query of this ApiRequestNotificationTypeResponse.  # noqa: E501
+        :return: The filter of this MatchingPattern.  # noqa: E501
         :rtype: str
         """
-        return self._path_and_query
+        return self._filter
 
-    @path_and_query.setter
-    def path_and_query(self, path_and_query):
-        """Sets the path_and_query of this ApiRequestNotificationTypeResponse.
-
-        The url to send the request to.  # noqa: E501
-
-        :param path_and_query: The path_and_query of this ApiRequestNotificationTypeResponse.  # noqa: E501
-        :type path_and_query: str
-        """
-
-        self._path_and_query = path_and_query
-
-    @property
-    def content(self):
-        """Gets the content of this ApiRequestNotificationTypeResponse.  # noqa: E501
-
-        The content of the request  # noqa: E501
-
-        :return: The content of this ApiRequestNotificationTypeResponse.  # noqa: E501
-        :rtype: object
-        """
-        return self._content
-
-    @content.setter
-    def content(self, content):
-        """Sets the content of this ApiRequestNotificationTypeResponse.
-
-        The content of the request  # noqa: E501
-
-        :param content: The content of this ApiRequestNotificationTypeResponse.  # noqa: E501
-        :type content: object
-        """
+    @filter.setter
+    def filter(self, filter):
+        """Sets the filter of this MatchingPattern.
+
+        A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched  # noqa: E501
+
+        :param filter: The filter of this MatchingPattern.  # noqa: E501
+        :type filter: str
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                filter is not None and len(filter) > 16384):
+            raise ValueError("Invalid value for `filter`, length must be less than or equal to `16384`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                filter is not None and len(filter) < 0):
+            raise ValueError("Invalid value for `filter`, length must be greater than or equal to `0`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                filter is not None and not re.search(r'^[\s\S]*$', filter)):  # noqa: E501
+            raise ValueError(r"Invalid value for `filter`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
-        self._content = content
+        self._filter = filter
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -217,18 +177,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ApiRequestNotificationTypeResponse):
+        if not isinstance(other, MatchingPattern):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ApiRequestNotificationTypeResponse):
+        if not isinstance(other, MatchingPattern):
             return True
 
         return self.to_dict() != other.to_dict()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/create_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/email_notification_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/email_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/email_notification_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/event_field_definition.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/event_field_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class IdentifierPartSchema(object):
+class ResourceListOfAccessControlledResource(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,220 +35,175 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'index': 'int',
-        'name': 'str',
-        'display_name': 'str',
-        'description': 'str',
-        'required': 'bool',
-        'links': 'list[Link]'
+        'values': 'list[AccessControlledResource]',
+        'href': 'str',
+        'links': 'list[Link]',
+        'next_page': 'str',
+        'previous_page': 'str'
     }
 
     attribute_map = {
-        'index': 'index',
-        'name': 'name',
-        'display_name': 'displayName',
-        'description': 'description',
-        'required': 'required',
-        'links': 'links'
+        'values': 'values',
+        'href': 'href',
+        'links': 'links',
+        'next_page': 'nextPage',
+        'previous_page': 'previousPage'
     }
 
     required_map = {
-        'index': 'required',
-        'name': 'required',
-        'display_name': 'required',
-        'description': 'required',
-        'required': 'required',
-        'links': 'optional'
+        'values': 'required',
+        'href': 'optional',
+        'links': 'optional',
+        'next_page': 'optional',
+        'previous_page': 'optional'
     }
 
-    def __init__(self, index=None, name=None, display_name=None, description=None, required=None, links=None, local_vars_configuration=None):  # noqa: E501
-        """IdentifierPartSchema - a model defined in OpenAPI"
+    def __init__(self, values=None, href=None, links=None, next_page=None, previous_page=None, local_vars_configuration=None):  # noqa: E501
+        """ResourceListOfAccessControlledResource - a model defined in OpenAPI"
         
-        :param index:  (required)
-        :type index: int
-        :param name:  (required)
-        :type name: str
-        :param display_name:  (required)
-        :type display_name: str
-        :param description:  (required)
-        :type description: str
-        :param required:  (required)
-        :type required: bool
+        :param values:  (required)
+        :type values: list[lusid_notification.AccessControlledResource]
+        :param href: 
+        :type href: str
         :param links: 
         :type links: list[lusid_notification.Link]
+        :param next_page: 
+        :type next_page: str
+        :param previous_page: 
+        :type previous_page: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._index = None
-        self._name = None
-        self._display_name = None
-        self._description = None
-        self._required = None
+        self._values = None
+        self._href = None
         self._links = None
+        self._next_page = None
+        self._previous_page = None
         self.discriminator = None
 
-        self.index = index
-        self.name = name
-        self.display_name = display_name
-        self.description = description
-        self.required = required
+        self.values = values
+        self.href = href
         self.links = links
+        self.next_page = next_page
+        self.previous_page = previous_page
 
     @property
-    def index(self):
-        """Gets the index of this IdentifierPartSchema.  # noqa: E501
+    def values(self):
+        """Gets the values of this ResourceListOfAccessControlledResource.  # noqa: E501
 
 
-        :return: The index of this IdentifierPartSchema.  # noqa: E501
-        :rtype: int
+        :return: The values of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :rtype: list[lusid_notification.AccessControlledResource]
         """
-        return self._index
+        return self._values
 
-    @index.setter
-    def index(self, index):
-        """Sets the index of this IdentifierPartSchema.
+    @values.setter
+    def values(self, values):
+        """Sets the values of this ResourceListOfAccessControlledResource.
 
 
-        :param index: The index of this IdentifierPartSchema.  # noqa: E501
-        :type index: int
+        :param values: The values of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :type values: list[lusid_notification.AccessControlledResource]
         """
-        if self.local_vars_configuration.client_side_validation and index is None:  # noqa: E501
-            raise ValueError("Invalid value for `index`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
+            raise ValueError("Invalid value for `values`, must not be `None`")  # noqa: E501
 
-        self._index = index
+        self._values = values
 
     @property
-    def name(self):
-        """Gets the name of this IdentifierPartSchema.  # noqa: E501
+    def href(self):
+        """Gets the href of this ResourceListOfAccessControlledResource.  # noqa: E501
 
 
-        :return: The name of this IdentifierPartSchema.  # noqa: E501
+        :return: The href of this ResourceListOfAccessControlledResource.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._href
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this IdentifierPartSchema.
+    @href.setter
+    def href(self, href):
+        """Sets the href of this ResourceListOfAccessControlledResource.
 
 
-        :param name: The name of this IdentifierPartSchema.  # noqa: E501
-        :type name: str
+        :param href: The href of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :type href: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                name is not None and len(name) < 1):
-            raise ValueError("Invalid value for `name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._name = name
+        self._href = href
 
     @property
-    def display_name(self):
-        """Gets the display_name of this IdentifierPartSchema.  # noqa: E501
+    def links(self):
+        """Gets the links of this ResourceListOfAccessControlledResource.  # noqa: E501
 
 
-        :return: The display_name of this IdentifierPartSchema.  # noqa: E501
-        :rtype: str
+        :return: The links of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :rtype: list[lusid_notification.Link]
         """
-        return self._display_name
+        return self._links
 
-    @display_name.setter
-    def display_name(self, display_name):
-        """Sets the display_name of this IdentifierPartSchema.
+    @links.setter
+    def links(self, links):
+        """Sets the links of this ResourceListOfAccessControlledResource.
 
 
-        :param display_name: The display_name of this IdentifierPartSchema.  # noqa: E501
-        :type display_name: str
+        :param links: The links of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :type links: list[lusid_notification.Link]
         """
-        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 1):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._display_name = display_name
+        self._links = links
 
     @property
-    def description(self):
-        """Gets the description of this IdentifierPartSchema.  # noqa: E501
+    def next_page(self):
+        """Gets the next_page of this ResourceListOfAccessControlledResource.  # noqa: E501
 
 
-        :return: The description of this IdentifierPartSchema.  # noqa: E501
+        :return: The next_page of this ResourceListOfAccessControlledResource.  # noqa: E501
         :rtype: str
         """
-        return self._description
-
-    @description.setter
-    def description(self, description):
-        """Sets the description of this IdentifierPartSchema.
-
-
-        :param description: The description of this IdentifierPartSchema.  # noqa: E501
-        :type description: str
-        """
-        if self.local_vars_configuration.client_side_validation and description is None:  # noqa: E501
-            raise ValueError("Invalid value for `description`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 1):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._description = description
-
-    @property
-    def required(self):
-        """Gets the required of this IdentifierPartSchema.  # noqa: E501
-
-
-        :return: The required of this IdentifierPartSchema.  # noqa: E501
-        :rtype: bool
-        """
-        return self._required
+        return self._next_page
 
-    @required.setter
-    def required(self, required):
-        """Sets the required of this IdentifierPartSchema.
+    @next_page.setter
+    def next_page(self, next_page):
+        """Sets the next_page of this ResourceListOfAccessControlledResource.
 
 
-        :param required: The required of this IdentifierPartSchema.  # noqa: E501
-        :type required: bool
+        :param next_page: The next_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :type next_page: str
         """
-        if self.local_vars_configuration.client_side_validation and required is None:  # noqa: E501
-            raise ValueError("Invalid value for `required`, must not be `None`")  # noqa: E501
 
-        self._required = required
+        self._next_page = next_page
 
     @property
-    def links(self):
-        """Gets the links of this IdentifierPartSchema.  # noqa: E501
+    def previous_page(self):
+        """Gets the previous_page of this ResourceListOfAccessControlledResource.  # noqa: E501
 
 
-        :return: The links of this IdentifierPartSchema.  # noqa: E501
-        :rtype: list[lusid_notification.Link]
+        :return: The previous_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :rtype: str
         """
-        return self._links
+        return self._previous_page
 
-    @links.setter
-    def links(self, links):
-        """Sets the links of this IdentifierPartSchema.
+    @previous_page.setter
+    def previous_page(self, previous_page):
+        """Sets the previous_page of this ResourceListOfAccessControlledResource.
 
 
-        :param links: The links of this IdentifierPartSchema.  # noqa: E501
-        :type links: list[lusid_notification.Link]
+        :param previous_page: The previous_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :type previous_page: str
         """
 
-        self._links = links
+        self._previous_page = previous_page
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -284,18 +239,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, IdentifierPartSchema):
+        if not isinstance(other, ResourceListOfAccessControlledResource):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, IdentifierPartSchema):
+        if not isinstance(other, ResourceListOfAccessControlledResource):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/manual_event_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/sms_notification_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class MatchingPattern(object):
+class SmsNotificationType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,113 +35,150 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'event_type': 'str',
-        'filter': 'str'
+        'type': 'str',
+        'body': 'str',
+        'recipients': 'list[str]'
     }
 
     attribute_map = {
-        'event_type': 'eventType',
-        'filter': 'filter'
+        'type': 'type',
+        'body': 'body',
+        'recipients': 'recipients'
     }
 
     required_map = {
-        'event_type': 'required',
-        'filter': 'optional'
+        'type': 'required',
+        'body': 'required',
+        'recipients': 'required'
     }
 
-    def __init__(self, event_type=None, filter=None, local_vars_configuration=None):  # noqa: E501
-        """MatchingPattern - a model defined in OpenAPI"
+    def __init__(self, type=None, body=None, recipients=None, local_vars_configuration=None):  # noqa: E501
+        """SmsNotificationType - a model defined in OpenAPI"
         
-        :param event_type:  The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint. (required)
-        :type event_type: str
-        :param filter:  A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched
-        :type filter: str
+        :param type:  The type of delivery mechanism for this notification (required)
+        :type type: str
+        :param body:  The body of the SMS (required)
+        :type body: str
+        :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
+        :type recipients: list[str]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
-        self._event_type = None
-        self._filter = None
+        self._type = None
+        self._body = None
+        self._recipients = None
         self.discriminator = None
 
-        self.event_type = event_type
-        self.filter = filter
+        self.type = type
+        self.body = body
+        self.recipients = recipients
 
     @property
-    def event_type(self):
-        """Gets the event_type of this MatchingPattern.  # noqa: E501
+    def type(self):
+        """Gets the type of this SmsNotificationType.  # noqa: E501
 
-        The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint.  # noqa: E501
+        The type of delivery mechanism for this notification  # noqa: E501
 
-        :return: The event_type of this MatchingPattern.  # noqa: E501
+        :return: The type of this SmsNotificationType.  # noqa: E501
         :rtype: str
         """
-        return self._event_type
+        return self._type
 
-    @event_type.setter
-    def event_type(self, event_type):
-        """Sets the event_type of this MatchingPattern.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this SmsNotificationType.
 
-        The type of event to subscribe to. The list of available event types can be discovered  by calling the ‘List available EventTypes’ API endpoint.  # noqa: E501
+        The type of delivery mechanism for this notification  # noqa: E501
 
-        :param event_type: The event_type of this MatchingPattern.  # noqa: E501
-        :type event_type: str
+        :param type: The type of this SmsNotificationType.  # noqa: E501
+        :type type: str
         """
-        if self.local_vars_configuration.client_side_validation and event_type is None:  # noqa: E501
-            raise ValueError("Invalid value for `event_type`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        allowed_values = ["Sms"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
+
+        self._type = type
+
+    @property
+    def body(self):
+        """Gets the body of this SmsNotificationType.  # noqa: E501
+
+        The body of the SMS  # noqa: E501
+
+        :return: The body of this SmsNotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._body
+
+    @body.setter
+    def body(self, body):
+        """Sets the body of this SmsNotificationType.
+
+        The body of the SMS  # noqa: E501
+
+        :param body: The body of this SmsNotificationType.  # noqa: E501
+        :type body: str
+        """
+        if self.local_vars_configuration.client_side_validation and body is None:  # noqa: E501
+            raise ValueError("Invalid value for `body`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                event_type is not None and len(event_type) > 512):
-            raise ValueError("Invalid value for `event_type`, length must be less than or equal to `512`")  # noqa: E501
+                body is not None and len(body) > 1024):
+            raise ValueError("Invalid value for `body`, length must be less than or equal to `1024`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                event_type is not None and len(event_type) < 0):
-            raise ValueError("Invalid value for `event_type`, length must be greater than or equal to `0`")  # noqa: E501
+                body is not None and len(body) < 1):
+            raise ValueError("Invalid value for `body`, length must be greater than or equal to `1`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                event_type is not None and not re.search(r'^[a-zA-Z]*$', event_type)):  # noqa: E501
-            raise ValueError(r"Invalid value for `event_type`, must be a follow pattern or equal to `/^[a-zA-Z]*$/`")  # noqa: E501
+                body is not None and not re.search(r'^[\s\S]*$', body)):  # noqa: E501
+            raise ValueError(r"Invalid value for `body`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
 
-        self._event_type = event_type
+        self._body = body
 
     @property
-    def filter(self):
-        """Gets the filter of this MatchingPattern.  # noqa: E501
+    def recipients(self):
+        """Gets the recipients of this SmsNotificationType.  # noqa: E501
 
-        A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched  # noqa: E501
+        The phone numbers to which the SMS will be sent to (E.164 format)  # noqa: E501
 
-        :return: The filter of this MatchingPattern.  # noqa: E501
-        :rtype: str
+        :return: The recipients of this SmsNotificationType.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._filter
+        return self._recipients
 
-    @filter.setter
-    def filter(self, filter):
-        """Sets the filter of this MatchingPattern.
+    @recipients.setter
+    def recipients(self, recipients):
+        """Sets the recipients of this SmsNotificationType.
 
-        A filter on the event. See https://support.lusid.com/filtering-results-from-lusid for more information. If not provided, all events will be matched  # noqa: E501
+        The phone numbers to which the SMS will be sent to (E.164 format)  # noqa: E501
 
-        :param filter: The filter of this MatchingPattern.  # noqa: E501
-        :type filter: str
+        :param recipients: The recipients of this SmsNotificationType.  # noqa: E501
+        :type recipients: list[str]
         """
+        if self.local_vars_configuration.client_side_validation and recipients is None:  # noqa: E501
+            raise ValueError("Invalid value for `recipients`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                filter is not None and len(filter) > 16384):
-            raise ValueError("Invalid value for `filter`, length must be less than or equal to `16384`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                filter is not None and len(filter) < 0):
-            raise ValueError("Invalid value for `filter`, length must be greater than or equal to `0`")  # noqa: E501
+                recipients is not None and len(recipients) > 10):
+            raise ValueError("Invalid value for `recipients`, number of items must be less than or equal to `10`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                filter is not None and not re.search(r'^[\s\S]*$', filter)):  # noqa: E501
-            raise ValueError(r"Invalid value for `filter`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
+                recipients is not None and len(recipients) < 1):
+            raise ValueError("Invalid value for `recipients`, number of items must be greater than or equal to `1`")  # noqa: E501
 
-        self._filter = filter
+        self._recipients = recipients
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -177,18 +214,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, MatchingPattern):
+        if not isinstance(other, SmsNotificationType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, MatchingPattern):
+        if not isinstance(other, SmsNotificationType):
             return True
 
         return self.to_dict() != other.to_dict()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -40,161 +40,154 @@
     """
     openapi_types = {
         'type': 'str',
         'api_key_ref': 'str',
         'api_secret_ref': 'str',
         'body': 'str',
         'queue_url_ref': 'str',
-        'http_method': 'str',
-        'path_and_query': 'str',
-        'content': 'object',
         'subject': 'str',
         'plain_text_body': 'str',
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]',
         'recipients': 'list[str]',
+        'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
         'authentication_configuration_item_paths': 'dict[str, str]',
-        'content_type': 'str'
+        'content_type': 'str',
+        'content': 'object'
     }
 
     attribute_map = {
         'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
         'body': 'body',
         'queue_url_ref': 'queueUrlRef',
-        'http_method': 'httpMethod',
-        'path_and_query': 'pathAndQuery',
-        'content': 'content',
         'subject': 'subject',
         'plain_text_body': 'plainTextBody',
         'html_body': 'htmlBody',
         'email_address_to': 'emailAddressTo',
         'email_address_cc': 'emailAddressCc',
         'email_address_bcc': 'emailAddressBcc',
         'recipients': 'recipients',
+        'http_method': 'httpMethod',
         'url': 'url',
         'authentication_type': 'authenticationType',
         'authentication_configuration_item_paths': 'authenticationConfigurationItemPaths',
-        'content_type': 'contentType'
+        'content_type': 'contentType',
+        'content': 'content'
     }
 
     required_map = {
         'type': 'required',
         'api_key_ref': 'required',
         'api_secret_ref': 'required',
         'body': 'required',
         'queue_url_ref': 'required',
-        'http_method': 'required',
-        'path_and_query': 'required',
-        'content': 'optional',
         'subject': 'required',
         'plain_text_body': 'required',
         'html_body': 'optional',
         'email_address_to': 'required',
         'email_address_cc': 'optional',
         'email_address_bcc': 'optional',
         'recipients': 'required',
+        'http_method': 'required',
         'url': 'required',
         'authentication_type': 'required',
         'authentication_configuration_item_paths': 'optional',
-        'content_type': 'required'
+        'content_type': 'required',
+        'content': 'optional'
     }
 
-    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, http_method=None, path_and_query=None, content=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
         """NotificationType - a model defined in OpenAPI"
         
         :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
         :param body:  The body of the SMS (required)
         :type body: str
         :param queue_url_ref:  Reference to queue url from Configuration Store (required)
         :type queue_url_ref: str
-        :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
-        :type http_method: str
-        :param path_and_query:  The url to send the request to. (required)
-        :type path_and_query: str
-        :param content:  The content of the request
-        :type content: object
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
+        :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
+        :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
+        :param content:  The content of the request
+        :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._api_key_ref = None
         self._api_secret_ref = None
         self._body = None
         self._queue_url_ref = None
-        self._http_method = None
-        self._path_and_query = None
-        self._content = None
         self._subject = None
         self._plain_text_body = None
         self._html_body = None
         self._email_address_to = None
         self._email_address_cc = None
         self._email_address_bcc = None
         self._recipients = None
+        self._http_method = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
+        self._content = None
         self.discriminator = None
 
         self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
-        self.http_method = http_method
-        self.path_and_query = path_and_query
-        self.content = content
         self.subject = subject
         self.plain_text_body = plain_text_body
         self.html_body = html_body
         self.email_address_to = email_address_to
         self.email_address_cc = email_address_cc
         self.email_address_bcc = email_address_bcc
         self.recipients = recipients
+        self.http_method = http_method
         self.url = url
         self.authentication_type = authentication_type
         self.authentication_configuration_item_paths = authentication_configuration_item_paths
         self.content_type = content_type
+        self.content = content
 
     @property
     def type(self):
         """Gets the type of this NotificationType.  # noqa: E501
 
         The type of delivery mechanism for this notification  # noqa: E501
 
@@ -338,99 +331,14 @@
         if (self.local_vars_configuration.client_side_validation and
                 queue_url_ref is not None and len(queue_url_ref) < 1):
             raise ValueError("Invalid value for `queue_url_ref`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._queue_url_ref = queue_url_ref
 
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
-    def path_and_query(self):
-        """Gets the path_and_query of this NotificationType.  # noqa: E501
-
-        The url to send the request to.  # noqa: E501
-
-        :return: The path_and_query of this NotificationType.  # noqa: E501
-        :rtype: str
-        """
-        return self._path_and_query
-
-    @path_and_query.setter
-    def path_and_query(self, path_and_query):
-        """Sets the path_and_query of this NotificationType.
-
-        The url to send the request to.  # noqa: E501
-
-        :param path_and_query: The path_and_query of this NotificationType.  # noqa: E501
-        :type path_and_query: str
-        """
-        if self.local_vars_configuration.client_side_validation and path_and_query is None:  # noqa: E501
-            raise ValueError("Invalid value for `path_and_query`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                path_and_query is not None and len(path_and_query) > 16384):
-            raise ValueError("Invalid value for `path_and_query`, length must be less than or equal to `16384`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                path_and_query is not None and len(path_and_query) < 1):
-            raise ValueError("Invalid value for `path_and_query`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                path_and_query is not None and not re.search(r'^([A-Za-z0-9-._~:\/?#[\]@!$&\'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$', path_and_query)):  # noqa: E501
-            raise ValueError(r"Invalid value for `path_and_query`, must be a follow pattern or equal to `/^([A-Za-z0-9-._~:\/?#[\]@!$&'()*+,;%=]|(\{\{([a-zA-Z0-9\s])*\}\}))*$/`")  # noqa: E501
-
-        self._path_and_query = path_and_query
-
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
-    @property
     def subject(self):
         """Gets the subject of this NotificationType.  # noqa: E501
 
         The subject of the email  # noqa: E501
 
         :return: The subject of this NotificationType.  # noqa: E501
         :rtype: str
@@ -637,14 +545,42 @@
         if (self.local_vars_configuration.client_side_validation and
                 recipients is not None and len(recipients) < 1):
             raise ValueError("Invalid value for `recipients`, number of items must be greater than or equal to `1`")  # noqa: E501
 
         self._recipients = recipients
 
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
     def url(self):
         """Gets the url of this NotificationType.  # noqa: E501
 
         The URL to send the request to  # noqa: E501
 
         :return: The url of this NotificationType.  # noqa: E501
         :rtype: str
@@ -749,14 +685,37 @@
             raise ValueError("Invalid value for `content_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 content_type is not None and len(content_type) < 1):
             raise ValueError("Invalid value for `content_type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._content_type = content_type
 
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
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/notification_type_response.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/notification_type_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -40,161 +40,154 @@
     """
     openapi_types = {
         'type': 'str',
         'api_key_ref': 'str',
         'api_secret_ref': 'str',
         'body': 'str',
         'queue_url_ref': 'str',
-        'http_method': 'str',
-        'path_and_query': 'str',
-        'content': 'object',
         'subject': 'str',
         'plain_text_body': 'str',
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]',
         'recipients': 'list[str]',
+        'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
         'authentication_configuration_item_paths': 'dict[str, str]',
-        'content_type': 'str'
+        'content_type': 'str',
+        'content': 'object'
     }
 
     attribute_map = {
         'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
         'body': 'body',
         'queue_url_ref': 'queueUrlRef',
-        'http_method': 'httpMethod',
-        'path_and_query': 'pathAndQuery',
-        'content': 'content',
         'subject': 'subject',
         'plain_text_body': 'plainTextBody',
         'html_body': 'htmlBody',
         'email_address_to': 'emailAddressTo',
         'email_address_cc': 'emailAddressCc',
         'email_address_bcc': 'emailAddressBcc',
         'recipients': 'recipients',
+        'http_method': 'httpMethod',
         'url': 'url',
         'authentication_type': 'authenticationType',
         'authentication_configuration_item_paths': 'authenticationConfigurationItemPaths',
-        'content_type': 'contentType'
+        'content_type': 'contentType',
+        'content': 'content'
     }
 
     required_map = {
         'type': 'optional',
         'api_key_ref': 'optional',
         'api_secret_ref': 'optional',
         'body': 'optional',
         'queue_url_ref': 'optional',
-        'http_method': 'optional',
-        'path_and_query': 'optional',
-        'content': 'optional',
         'subject': 'optional',
         'plain_text_body': 'optional',
         'html_body': 'optional',
         'email_address_to': 'optional',
         'email_address_cc': 'optional',
         'email_address_bcc': 'optional',
         'recipients': 'optional',
+        'http_method': 'optional',
         'url': 'optional',
         'authentication_type': 'optional',
         'authentication_configuration_item_paths': 'optional',
-        'content_type': 'optional'
+        'content_type': 'optional',
+        'content': 'optional'
     }
 
-    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, http_method=None, path_and_query=None, content=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
         """NotificationTypeResponse - a model defined in OpenAPI"
         
         :param type:  The type of delivery mechanism for this notification
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store
         :type api_secret_ref: str
         :param body:  The body of the SMS
         :type body: str
         :param queue_url_ref:  Reference to queue url from Configuration Store
         :type queue_url_ref: str
-        :param http_method:  The HTTP method such as GET, POST, etc. to use on the request
-        :type http_method: str
-        :param path_and_query:  The url to send the request to.
-        :type path_and_query: str
-        :param content:  The content of the request
-        :type content: object
         :param subject:  The subject of the email
         :type subject: str
         :param plain_text_body:  The plain text body of the email
         :type plain_text_body: str
         :param html_body:  The HTML body of the email (if any)
         :type html_body: str
         :param email_address_to:  'To' recipients of the email
         :type email_address_to: list[str]
         :param email_address_cc:  'Cc' recipients of the email
         :type email_address_cc: list[str]
         :param email_address_bcc:  'Bcc' recipients of the email
         :type email_address_bcc: list[str]
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format)
         :type recipients: list[str]
+        :param http_method:  The HTTP method such as GET, POST, etc. to use on the request
+        :type http_method: str
         :param url:  The URL to send the request to
         :type url: str
         :param authentication_type:  The type of authentication to use on the request
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
         :type authentication_configuration_item_paths: dict[str, str]
         :param content_type:  The type of the content e.g. Json
         :type content_type: str
+        :param content:  The content of the request
+        :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._type = None
         self._api_key_ref = None
         self._api_secret_ref = None
         self._body = None
         self._queue_url_ref = None
-        self._http_method = None
-        self._path_and_query = None
-        self._content = None
         self._subject = None
         self._plain_text_body = None
         self._html_body = None
         self._email_address_to = None
         self._email_address_cc = None
         self._email_address_bcc = None
         self._recipients = None
+        self._http_method = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
+        self._content = None
         self.discriminator = None
 
         self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
-        self.http_method = http_method
-        self.path_and_query = path_and_query
-        self.content = content
         self.subject = subject
         self.plain_text_body = plain_text_body
         self.html_body = html_body
         self.email_address_to = email_address_to
         self.email_address_cc = email_address_cc
         self.email_address_bcc = email_address_bcc
         self.recipients = recipients
+        self.http_method = http_method
         self.url = url
         self.authentication_type = authentication_type
         self.authentication_configuration_item_paths = authentication_configuration_item_paths
         self.content_type = content_type
+        self.content = content
 
     @property
     def type(self):
         """Gets the type of this NotificationTypeResponse.  # noqa: E501
 
         The type of delivery mechanism for this notification  # noqa: E501
 
@@ -304,83 +297,14 @@
         :param queue_url_ref: The queue_url_ref of this NotificationTypeResponse.  # noqa: E501
         :type queue_url_ref: str
         """
 
         self._queue_url_ref = queue_url_ref
 
     @property
-    def http_method(self):
-        """Gets the http_method of this NotificationTypeResponse.  # noqa: E501
-
-        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
-
-        :return: The http_method of this NotificationTypeResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._http_method
-
-    @http_method.setter
-    def http_method(self, http_method):
-        """Sets the http_method of this NotificationTypeResponse.
-
-        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
-
-        :param http_method: The http_method of this NotificationTypeResponse.  # noqa: E501
-        :type http_method: str
-        """
-
-        self._http_method = http_method
-
-    @property
-    def path_and_query(self):
-        """Gets the path_and_query of this NotificationTypeResponse.  # noqa: E501
-
-        The url to send the request to.  # noqa: E501
-
-        :return: The path_and_query of this NotificationTypeResponse.  # noqa: E501
-        :rtype: str
-        """
-        return self._path_and_query
-
-    @path_and_query.setter
-    def path_and_query(self, path_and_query):
-        """Sets the path_and_query of this NotificationTypeResponse.
-
-        The url to send the request to.  # noqa: E501
-
-        :param path_and_query: The path_and_query of this NotificationTypeResponse.  # noqa: E501
-        :type path_and_query: str
-        """
-
-        self._path_and_query = path_and_query
-
-    @property
-    def content(self):
-        """Gets the content of this NotificationTypeResponse.  # noqa: E501
-
-        The content of the request  # noqa: E501
-
-        :return: The content of this NotificationTypeResponse.  # noqa: E501
-        :rtype: object
-        """
-        return self._content
-
-    @content.setter
-    def content(self, content):
-        """Sets the content of this NotificationTypeResponse.
-
-        The content of the request  # noqa: E501
-
-        :param content: The content of this NotificationTypeResponse.  # noqa: E501
-        :type content: object
-        """
-
-        self._content = content
-
-    @property
     def subject(self):
         """Gets the subject of this NotificationTypeResponse.  # noqa: E501
 
         The subject of the email  # noqa: E501
 
         :return: The subject of this NotificationTypeResponse.  # noqa: E501
         :rtype: str
@@ -534,14 +458,37 @@
         :param recipients: The recipients of this NotificationTypeResponse.  # noqa: E501
         :type recipients: list[str]
         """
 
         self._recipients = recipients
 
     @property
+    def http_method(self):
+        """Gets the http_method of this NotificationTypeResponse.  # noqa: E501
+
+        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
+
+        :return: The http_method of this NotificationTypeResponse.  # noqa: E501
+        :rtype: str
+        """
+        return self._http_method
+
+    @http_method.setter
+    def http_method(self, http_method):
+        """Sets the http_method of this NotificationTypeResponse.
+
+        The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
+
+        :param http_method: The http_method of this NotificationTypeResponse.  # noqa: E501
+        :type http_method: str
+        """
+
+        self._http_method = http_method
+
+    @property
     def url(self):
         """Gets the url of this NotificationTypeResponse.  # noqa: E501
 
         The URL to send the request to  # noqa: E501
 
         :return: The url of this NotificationTypeResponse.  # noqa: E501
         :rtype: str
@@ -625,14 +572,37 @@
 
         :param content_type: The content_type of this NotificationTypeResponse.  # noqa: E501
         :type content_type: str
         """
 
         self._content_type = content_type
 
+    @property
+    def content(self):
+        """Gets the content of this NotificationTypeResponse.  # noqa: E501
+
+        The content of the request  # noqa: E501
+
+        :return: The content of this NotificationTypeResponse.  # noqa: E501
+        :rtype: object
+        """
+        return self._content
+
+    @content.setter
+    def content(self, content):
+        """Sets the content of this NotificationTypeResponse.
+
+        The content of the request  # noqa: E501
+
+        :param content: The content of this NotificationTypeResponse.  # noqa: E501
+        :type content: object
+        """
+
+        self._content = content
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class ResourceListOfAccessControlledResource(object):
+class ResourceListOfEventTypeSchema(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,15 +35,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'values': 'list[AccessControlledResource]',
+        'values': 'list[EventTypeSchema]',
         'href': 'str',
         'links': 'list[Link]',
         'next_page': 'str',
         'previous_page': 'str'
     }
 
     attribute_map = {
@@ -59,18 +59,18 @@
         'href': 'optional',
         'links': 'optional',
         'next_page': 'optional',
         'previous_page': 'optional'
     }
 
     def __init__(self, values=None, href=None, links=None, next_page=None, previous_page=None, local_vars_configuration=None):  # noqa: E501
-        """ResourceListOfAccessControlledResource - a model defined in OpenAPI"
+        """ResourceListOfEventTypeSchema - a model defined in OpenAPI"
         
         :param values:  (required)
-        :type values: list[lusid_notification.AccessControlledResource]
+        :type values: list[lusid_notification.EventTypeSchema]
         :param href: 
         :type href: str
         :param links: 
         :type links: list[lusid_notification.Link]
         :param next_page: 
         :type next_page: str
         :param previous_page: 
@@ -92,114 +92,114 @@
         self.href = href
         self.links = links
         self.next_page = next_page
         self.previous_page = previous_page
 
     @property
     def values(self):
-        """Gets the values of this ResourceListOfAccessControlledResource.  # noqa: E501
+        """Gets the values of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The values of this ResourceListOfAccessControlledResource.  # noqa: E501
-        :rtype: list[lusid_notification.AccessControlledResource]
+        :return: The values of this ResourceListOfEventTypeSchema.  # noqa: E501
+        :rtype: list[lusid_notification.EventTypeSchema]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this ResourceListOfAccessControlledResource.
+        """Sets the values of this ResourceListOfEventTypeSchema.
 
 
-        :param values: The values of this ResourceListOfAccessControlledResource.  # noqa: E501
-        :type values: list[lusid_notification.AccessControlledResource]
+        :param values: The values of this ResourceListOfEventTypeSchema.  # noqa: E501
+        :type values: list[lusid_notification.EventTypeSchema]
         """
         if self.local_vars_configuration.client_side_validation and values is None:  # noqa: E501
             raise ValueError("Invalid value for `values`, must not be `None`")  # noqa: E501
 
         self._values = values
 
     @property
     def href(self):
-        """Gets the href of this ResourceListOfAccessControlledResource.  # noqa: E501
+        """Gets the href of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The href of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :return: The href of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: str
         """
         return self._href
 
     @href.setter
     def href(self, href):
-        """Sets the href of this ResourceListOfAccessControlledResource.
+        """Sets the href of this ResourceListOfEventTypeSchema.
 
 
-        :param href: The href of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :param href: The href of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type href: str
         """
 
         self._href = href
 
     @property
     def links(self):
-        """Gets the links of this ResourceListOfAccessControlledResource.  # noqa: E501
+        """Gets the links of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The links of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :return: The links of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: list[lusid_notification.Link]
         """
         return self._links
 
     @links.setter
     def links(self, links):
-        """Sets the links of this ResourceListOfAccessControlledResource.
+        """Sets the links of this ResourceListOfEventTypeSchema.
 
 
-        :param links: The links of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :param links: The links of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type links: list[lusid_notification.Link]
         """
 
         self._links = links
 
     @property
     def next_page(self):
-        """Gets the next_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        """Gets the next_page of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The next_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :return: The next_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: str
         """
         return self._next_page
 
     @next_page.setter
     def next_page(self, next_page):
-        """Sets the next_page of this ResourceListOfAccessControlledResource.
+        """Sets the next_page of this ResourceListOfEventTypeSchema.
 
 
-        :param next_page: The next_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :param next_page: The next_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type next_page: str
         """
 
         self._next_page = next_page
 
     @property
     def previous_page(self):
-        """Gets the previous_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        """Gets the previous_page of this ResourceListOfEventTypeSchema.  # noqa: E501
 
 
-        :return: The previous_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :return: The previous_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :rtype: str
         """
         return self._previous_page
 
     @previous_page.setter
     def previous_page(self, previous_page):
-        """Sets the previous_page of this ResourceListOfAccessControlledResource.
+        """Sets the previous_page of this ResourceListOfEventTypeSchema.
 
 
-        :param previous_page: The previous_page of this ResourceListOfAccessControlledResource.  # noqa: E501
+        :param previous_page: The previous_page of this ResourceListOfEventTypeSchema.  # noqa: E501
         :type previous_page: str
         """
 
         self._previous_page = previous_page
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
@@ -239,18 +239,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResourceListOfAccessControlledResource):
+        if not isinstance(other, ResourceListOfEventTypeSchema):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ResourceListOfAccessControlledResource):
+        if not isinstance(other, ResourceListOfEventTypeSchema):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/sms_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/sms_notification_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/webhook_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/models/webhook_notification_type_response.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/models/webhook_notification_type_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.772.5
+    The version of the OpenAPI document: 0.1.772.6
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.772.5/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.772.6/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 lusid_notification/api/subscriptions_api.py
 lusid_notification/models/__init__.py
 lusid_notification/models/access_controlled_action.py
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
 lusid_notification/models/amazon_sqs_notification_type_response.py
-lusid_notification/models/api_request_notification_type.py
-lusid_notification/models/api_request_notification_type_response.py
 lusid_notification/models/create_notification_request.py
 lusid_notification/models/create_subscription.py
 lusid_notification/models/email_notification_type.py
 lusid_notification/models/email_notification_type_response.py
 lusid_notification/models/event_field_definition.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
```

### Comparing `lusid-notification-sdk-preview-0.1.772.5/setup.py` & `lusid-notification-sdk-preview-0.1.772.6/setup.py`

 * *Files identical despite different names*

