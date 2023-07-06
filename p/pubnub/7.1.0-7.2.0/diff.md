# Comparing `tmp/pubnub-7.1.0.tar.gz` & `tmp/pubnub-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubnub-7.1.0.tar", last modified: Tue Jan 17 08:05:41 2023, max compression
+gzip compressed data, was "pubnub-7.2.0.tar", last modified: Thu Jul  6 09:45:14 2023, max compression
```

## Comparing `pubnub-7.1.0.tar` & `pubnub-7.2.0.tar`

### file list

```diff
@@ -1,189 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.125702 pubnub-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-01-17 08:05:24.000000 pubnub-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-17 08:05:41.125702 pubnub-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-01-17 08:05:24.000000 pubnub-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.101701 pubnub-7.1.0/pubnub/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/crypto_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/dtos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.105702 pubnub-7.1.0/pubnub/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.105702 pubnub-7.1.0/pubnub/endpoints/access/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/access/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/access/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/access/grant_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/access/revoke_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.105702 pubnub-7.1.0/pubnub/endpoints/channel_groups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/channel_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/channel_groups/remove_channel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.105702 pubnub-7.1.0/pubnub/endpoints/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.105702 pubnub-7.1.0/pubnub/endpoints/entities/membership/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/membership/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/membership/add_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/membership/fetch_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/membership/remove_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/membership/update_memberships.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.109701 pubnub-7.1.0/pubnub/endpoints/entities/space/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/space/create_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/space/fetch_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/space/fetch_spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/space/remove_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/space/update_space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.109701 pubnub-7.1.0/pubnub/endpoints/entities/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/user/create_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/user/fetch_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/user/fetch_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/user/remove_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/entities/user/update_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/fetch_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.109701 pubnub-7.1.0/pubnub/endpoints/file_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/download_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/download_file_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/fetch_upload_details.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/file_based_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/list_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/publish_file_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/send_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/file_operations/send_file_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/history_delete.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.109701 pubnub-7.1.0/pubnub/endpoints/message_actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/message_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/message_actions/add_message_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/message_actions/get_message_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/message_actions/remove_message_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/message_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.109701 pubnub-7.1.0/pubnub/endpoints/objects_v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.113701 pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/get_all_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/get_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/remove_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/set_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.113701 pubnub-7.1.0/pubnub/endpoints/objects_v2/members/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/members/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/members/get_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/members/manage_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/members/remove_channel_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/members/set_channel_members.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.113701 pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/get_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/manage_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/remove_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/set_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/objects_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.113701 pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/get_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/remove_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/set_uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.117701 pubnub-7.1.0/pubnub/endpoints/presence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/get_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/here_now.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/leave.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/set_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/presence/where_now.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.117701 pubnub-7.1.0/pubnub/endpoints/pubsub/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/pubsub/fire.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/pubsub/subscribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.117701 pubnub-7.1.0/pubnub/endpoints/push/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/push/add_channels_to_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/push/list_push_provisions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/push/remove_channels_from_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/push/remove_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/endpoints/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/features.py
--rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.117701 pubnub-7.1.0/pubnub/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.117701 pubnub-7.1.0/pubnub/models/consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/access_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/channel_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.121702 pubnub-7.1.0/pubnub/models/consumer/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/entities/membership.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/entities/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/entities/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/entities/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/message_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/message_count.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.121702 pubnub-7.1.0/pubnub/models/consumer/objects_v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/channel_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/objects_v2/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/pn_error_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/push.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.121702 pubnub-7.1.0/pubnub/models/consumer/v3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/access_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/pn_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/space.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/consumer/v3/uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.121702 pubnub-7.1.0/pubnub/models/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/server/subscribe.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/models/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/pnconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/pubnub.py
--rw-r--r--   0 runner    (1001) docker     (123)    24819 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/pubnub_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/pubnub_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.125702 pubnub-7.1.0/pubnub/request_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/request_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/request_handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/request_handlers/requests_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-01-17 08:05:24.000000 pubnub-7.1.0/pubnub/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:05:41.101701 pubnub-7.1.0/pubnub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-17 08:05:41.000000 pubnub-7.1.0/pubnub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-01-17 08:05:41.000000 pubnub-7.1.0/pubnub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:05:41.000000 pubnub-7.1.0/pubnub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:05:41.000000 pubnub-7.1.0/pubnub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-17 08:05:41.000000 pubnub-7.1.0/pubnub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-17 08:05:41.000000 pubnub-7.1.0/pubnub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-17 08:05:41.125702 pubnub-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-01-17 08:05:24.000000 pubnub-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.476954 pubnub-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-06 09:44:54.000000 pubnub-7.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-06 09:45:14.476954 pubnub-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-06 09:44:54.000000 pubnub-7.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.452954 pubnub-7.2.0/pubnub/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/crypto_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/dtos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.452954 pubnub-7.2.0/pubnub/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.452954 pubnub-7.2.0/pubnub/endpoints/access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/access/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/access/grant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/access/grant_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/access/revoke_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.456954 pubnub-7.2.0/pubnub/endpoints/channel_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/channel_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/channel_groups/remove_channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.456954 pubnub-7.2.0/pubnub/endpoints/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.456954 pubnub-7.2.0/pubnub/endpoints/entities/membership/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/membership/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/membership/add_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/membership/fetch_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/membership/remove_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/membership/update_memberships.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.456954 pubnub-7.2.0/pubnub/endpoints/entities/space/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/space/create_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/space/fetch_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/space/fetch_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/space/remove_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/space/update_space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.460954 pubnub-7.2.0/pubnub/endpoints/entities/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/user/create_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/user/fetch_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/user/fetch_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/user/remove_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/entities/user/update_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/fetch_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.460954 pubnub-7.2.0/pubnub/endpoints/file_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/download_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/download_file_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/fetch_upload_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/file_based_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/publish_file_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/send_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/file_operations/send_file_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/history_delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.460954 pubnub-7.2.0/pubnub/endpoints/message_actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/message_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/message_actions/add_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/message_actions/get_message_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/message_actions/remove_message_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/message_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.460954 pubnub-7.2.0/pubnub/endpoints/objects_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.464954 pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/get_all_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/get_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/remove_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/set_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.464954 pubnub-7.2.0/pubnub/endpoints/objects_v2/members/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/members/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/members/get_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/members/manage_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/members/remove_channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/members/set_channel_members.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.464954 pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/get_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/manage_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/remove_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/set_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/objects_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.464954 pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/get_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/remove_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/set_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.468954 pubnub-7.2.0/pubnub/endpoints/presence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/get_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/here_now.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/leave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/set_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/presence/where_now.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.468954 pubnub-7.2.0/pubnub/endpoints/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/pubsub/fire.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/pubsub/subscribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.468954 pubnub-7.2.0/pubnub/endpoints/push/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/push/add_channels_to_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/push/list_push_provisions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/push/remove_channels_from_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/push/remove_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/endpoints/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.468954 pubnub-7.2.0/pubnub/event_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/event_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/event_engine/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/event_engine/effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/event_engine/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/event_engine/statemachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/event_engine/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19618 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.468954 pubnub-7.2.0/pubnub/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.472954 pubnub-7.2.0/pubnub/models/consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/access_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/channel_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.472954 pubnub-7.2.0/pubnub/models/consumer/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/entities/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/entities/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/entities/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/entities/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/message_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/message_count.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.476954 pubnub-7.2.0/pubnub/models/consumer/objects_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/channel_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/objects_v2/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/pn_error_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.476954 pubnub-7.2.0/pubnub/models/consumer/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/access_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/pn_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/consumer/v3/uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.476954 pubnub-7.2.0/pubnub/models/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/server/subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/models/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/pnconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/pubnub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24871 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/pubnub_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20194 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/pubnub_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.476954 pubnub-7.2.0/pubnub/request_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/request_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/request_handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11701 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/request_handlers/requests_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-06 09:44:54.000000 pubnub-7.2.0/pubnub/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 09:45:14.452954 pubnub-7.2.0/pubnub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-06 09:45:14.000000 pubnub-7.2.0/pubnub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-06 09:45:14.000000 pubnub-7.2.0/pubnub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:45:14.000000 pubnub-7.2.0/pubnub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 09:45:14.000000 pubnub-7.2.0/pubnub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 09:45:14.000000 pubnub-7.2.0/pubnub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 09:45:14.000000 pubnub-7.2.0/pubnub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 09:45:14.476954 pubnub-7.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-06 09:44:54.000000 pubnub-7.2.0/setup.py
```

### Comparing `pubnub-7.1.0/LICENSE` & `pubnub-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/PKG-INFO` & `pubnub-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubnub
-Version: 7.1.0
+Version: 7.2.0
 Summary: PubNub Real-time push service in the cloud
 Home-page: http://pubnub.com
 Author: PubNub
 Author-email: support@pubnub.com
 License: MIT
 Project-URL: Source, https://github.com/pubnub/python
 Project-URL: Documentation, https://www.pubnub.com/docs/sdks/python
```

### Comparing `pubnub-7.1.0/README.md` & `pubnub-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/__init__.py` & `pubnub-7.2.0/pubnub/__init__.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/builders.py` & `pubnub-7.2.0/pubnub/builders.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/callbacks.py` & `pubnub-7.2.0/pubnub/callbacks.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/crypto.py` & `pubnub-7.2.0/pubnub/crypto.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 import hashlib
 import json
 import random
 from base64 import decodebytes, encodebytes
 
-from .crypto_core import PubNubCrypto
+from pubnub.crypto_core import PubNubCrypto
 from Cryptodome.Cipher import AES
 from Cryptodome.Util.Padding import pad, unpad
 
 
 Initial16bytes = '0123456789012345'
 
 
 class PubNubCryptodome(PubNubCrypto):
+    mode = AES.MODE_CBC
+    fallback_mode = None
+
     def __init__(self, pubnub_config):
         self.pubnub_configuration = pubnub_config
+        self.mode = pubnub_config.cipher_mode
+        self.fallback_mode = pubnub_config.fallback_cipher_mode
 
     def encrypt(self, key, msg, use_random_iv=False):
         secret = self.get_secret(key)
         initialization_vector = self.get_initialization_vector(use_random_iv)
 
-        cipher = AES.new(bytes(secret[0:32], 'utf-8'), AES.MODE_CBC, bytes(initialization_vector, 'utf-8'))
+        cipher = AES.new(bytes(secret[0:32], 'utf-8'), self.mode, bytes(initialization_vector, 'utf-8'))
         encrypted_message = cipher.encrypt(self.pad(msg.encode('utf-8')))
         msg_with_iv = self.append_random_iv(encrypted_message, use_random_iv, bytes(initialization_vector, "utf-8"))
 
         return encodebytes(msg_with_iv).decode('utf-8').replace("\n", "")
 
     def decrypt(self, key, msg, use_random_iv=False):
         secret = self.get_secret(key)
 
         decoded_message = decodebytes(msg.encode("utf-8"))
         initialization_vector, extracted_message = self.extract_random_iv(decoded_message, use_random_iv)
-        cipher = AES.new(bytes(secret[0:32], "utf-8"), AES.MODE_CBC, initialization_vector)
-        plain = self.depad((cipher.decrypt(extracted_message)).decode('utf-8'))
+        cipher = AES.new(bytes(secret[0:32], "utf-8"), self.mode, initialization_vector)
+        try:
+            plain = self.depad((cipher.decrypt(extracted_message)).decode('utf-8'))
+        except UnicodeDecodeError as e:
+            if not self.fallback_mode:
+                raise e
+
+            cipher = AES.new(bytes(secret[0:32], "utf-8"), self.fallback_mode, initialization_vector)
+            plain = self.depad((cipher.decrypt(extracted_message)).decode('utf-8'))
 
         try:
             return json.loads(plain)
         except Exception:
             return plain
 
     def append_random_iv(self, message, use_random_iv, initialization_vector):
@@ -67,22 +79,27 @@
         return hashlib.sha256(key.encode("utf-8")).hexdigest()
 
 
 class PubNubFileCrypto(PubNubCryptodome):
     def encrypt(self, key, file):
         secret = self.get_secret(key)
         initialization_vector = self.get_initialization_vector(use_random_iv=True)
-        cipher = AES.new(bytes(secret[0:32], "utf-8"), AES.MODE_CBC, bytes(initialization_vector, 'utf-8'))
+        cipher = AES.new(bytes(secret[0:32], "utf-8"), self.mode, bytes(initialization_vector, 'utf-8'))
         initialization_vector = bytes(initialization_vector, 'utf-8')
 
         return self.append_random_iv(
             cipher.encrypt(pad(file, 16)),
             use_random_iv=True,
             initialization_vector=initialization_vector
         )
 
     def decrypt(self, key, file):
         secret = self.get_secret(key)
         initialization_vector, extracted_file = self.extract_random_iv(file, use_random_iv=True)
-        cipher = AES.new(bytes(secret[0:32], "utf-8"), AES.MODE_CBC, initialization_vector)
+        try:
+            cipher = AES.new(bytes(secret[0:32], "utf-8"), self.mode, initialization_vector)
+            result = unpad(cipher.decrypt(extracted_file), 16)
+        except ValueError:
+            cipher = AES.new(bytes(secret[0:32], "utf-8"), self.fallback_mode, initialization_vector)
+            result = unpad(cipher.decrypt(extracted_file), 16)
 
-        return unpad(cipher.decrypt(extracted_file), 16)
+        return result
```

### Comparing `pubnub-7.1.0/pubnub/dtos.py` & `pubnub-7.2.0/pubnub/dtos.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/access/audit.py` & `pubnub-7.2.0/pubnub/endpoints/access/audit.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/access/grant.py` & `pubnub-7.2.0/pubnub/endpoints/access/grant.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/access/grant_token.py` & `pubnub-7.2.0/pubnub/endpoints/access/grant_token.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/access/revoke_token.py` & `pubnub-7.2.0/pubnub/endpoints/access/revoke_token.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py` & `pubnub-7.2.0/pubnub/endpoints/channel_groups/add_channel_to_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py` & `pubnub-7.2.0/pubnub/endpoints/channel_groups/list_channels_in_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py` & `pubnub-7.2.0/pubnub/endpoints/channel_groups/remove_channel_from_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/channel_groups/remove_channel_group.py` & `pubnub-7.2.0/pubnub/endpoints/channel_groups/remove_channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/endpoint.py` & `pubnub-7.2.0/pubnub/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/endpoint.py` & `pubnub-7.2.0/pubnub/endpoints/entities/endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/membership/add_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/entities/membership/add_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/membership/fetch_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/entities/membership/fetch_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/membership/remove_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/entities/membership/remove_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/membership/update_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/entities/membership/update_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/space/create_space.py` & `pubnub-7.2.0/pubnub/endpoints/entities/space/create_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/space/fetch_space.py` & `pubnub-7.2.0/pubnub/endpoints/entities/space/fetch_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/space/fetch_spaces.py` & `pubnub-7.2.0/pubnub/endpoints/entities/space/fetch_spaces.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/space/remove_space.py` & `pubnub-7.2.0/pubnub/endpoints/entities/space/remove_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/space/update_space.py` & `pubnub-7.2.0/pubnub/endpoints/entities/space/update_space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/user/create_user.py` & `pubnub-7.2.0/pubnub/endpoints/entities/user/create_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/user/fetch_user.py` & `pubnub-7.2.0/pubnub/endpoints/entities/user/fetch_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/user/fetch_users.py` & `pubnub-7.2.0/pubnub/endpoints/entities/user/fetch_users.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/user/remove_user.py` & `pubnub-7.2.0/pubnub/endpoints/entities/user/remove_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/entities/user/update_user.py` & `pubnub-7.2.0/pubnub/endpoints/entities/user/update_user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/fetch_messages.py` & `pubnub-7.2.0/pubnub/endpoints/fetch_messages.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/delete_file.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/delete_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/download_file.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/download_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/download_file_asyncio.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/download_file_asyncio.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/fetch_upload_details.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/fetch_upload_details.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/get_file_url.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/get_file_url.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/list_files.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/list_files.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/publish_file_message.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/publish_file_message.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/send_file.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/send_file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/file_operations/send_file_asyncio.py` & `pubnub-7.2.0/pubnub/endpoints/file_operations/send_file_asyncio.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/history.py` & `pubnub-7.2.0/pubnub/endpoints/history.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/history_delete.py` & `pubnub-7.2.0/pubnub/endpoints/history_delete.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/message_actions/add_message_action.py` & `pubnub-7.2.0/pubnub/endpoints/message_actions/add_message_action.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/message_actions/get_message_actions.py` & `pubnub-7.2.0/pubnub/endpoints/message_actions/get_message_actions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/message_actions/remove_message_action.py` & `pubnub-7.2.0/pubnub/endpoints/message_actions/remove_message_action.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/message_count.py` & `pubnub-7.2.0/pubnub/endpoints/message_count.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/mixins.py` & `pubnub-7.2.0/pubnub/endpoints/mixins.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/get_all_channels.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/get_all_channels.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/get_channel.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/get_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/remove_channel.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/remove_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/channel/set_channel.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/channel/set_channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/members/get_channel_members.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/members/get_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/members/manage_channel_members.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/members/manage_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/members/remove_channel_members.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/members/remove_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/members/set_channel_members.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/members/set_channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/get_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/get_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/manage_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/manage_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/remove_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/remove_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/memberships/set_memberships.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/memberships/set_memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/objects_endpoint.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/objects_endpoint.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/get_all_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/get_uuid.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/get_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/remove_uuid.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/remove_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/objects_v2/uuid/set_uuid.py` & `pubnub-7.2.0/pubnub/endpoints/objects_v2/uuid/set_uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/presence/get_state.py` & `pubnub-7.2.0/pubnub/endpoints/presence/get_state.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/presence/heartbeat.py` & `pubnub-7.2.0/pubnub/endpoints/presence/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/presence/here_now.py` & `pubnub-7.2.0/pubnub/endpoints/presence/here_now.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/presence/leave.py` & `pubnub-7.2.0/pubnub/endpoints/presence/leave.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/presence/set_state.py` & `pubnub-7.2.0/pubnub/endpoints/presence/set_state.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/presence/where_now.py` & `pubnub-7.2.0/pubnub/endpoints/presence/where_now.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/pubsub/fire.py` & `pubnub-7.2.0/pubnub/endpoints/pubsub/fire.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/pubsub/publish.py` & `pubnub-7.2.0/pubnub/endpoints/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/pubsub/subscribe.py` & `pubnub-7.2.0/pubnub/endpoints/pubsub/subscribe.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/push/add_channels_to_push.py` & `pubnub-7.2.0/pubnub/endpoints/push/add_channels_to_push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/push/list_push_provisions.py` & `pubnub-7.2.0/pubnub/endpoints/push/list_push_provisions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/push/remove_channels_from_push.py` & `pubnub-7.2.0/pubnub/endpoints/push/remove_channels_from_push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/push/remove_device.py` & `pubnub-7.2.0/pubnub/endpoints/push/remove_device.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/signal.py` & `pubnub-7.2.0/pubnub/endpoints/signal.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/endpoints/time.py` & `pubnub-7.2.0/pubnub/endpoints/time.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/enums.py` & `pubnub-7.2.0/pubnub/enums.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/errors.py` & `pubnub-7.2.0/pubnub/errors.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/exceptions.py` & `pubnub-7.2.0/pubnub/exceptions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/managers.py` & `pubnub-7.2.0/pubnub/managers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/access_manager.py` & `pubnub-7.2.0/pubnub/models/consumer/access_manager.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/channel_group.py` & `pubnub-7.2.0/pubnub/models/consumer/channel_group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/common.py` & `pubnub-7.2.0/pubnub/models/consumer/common.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/entities/membership.py` & `pubnub-7.2.0/pubnub/models/consumer/entities/membership.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/entities/page.py` & `pubnub-7.2.0/pubnub/models/consumer/entities/page.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/entities/space.py` & `pubnub-7.2.0/pubnub/models/consumer/entities/space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/entities/user.py` & `pubnub-7.2.0/pubnub/models/consumer/entities/user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/file.py` & `pubnub-7.2.0/pubnub/models/consumer/file.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/history.py` & `pubnub-7.2.0/pubnub/models/consumer/history.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/message_actions.py` & `pubnub-7.2.0/pubnub/models/consumer/message_actions.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/objects_v2/channel.py` & `pubnub-7.2.0/pubnub/models/consumer/objects_v2/channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/objects_v2/channel_members.py` & `pubnub-7.2.0/pubnub/models/consumer/objects_v2/channel_members.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/objects_v2/memberships.py` & `pubnub-7.2.0/pubnub/models/consumer/objects_v2/memberships.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/objects_v2/page.py` & `pubnub-7.2.0/pubnub/models/consumer/objects_v2/page.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/objects_v2/sort.py` & `pubnub-7.2.0/pubnub/models/consumer/objects_v2/sort.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/objects_v2/uuid.py` & `pubnub-7.2.0/pubnub/models/consumer/objects_v2/uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/presence.py` & `pubnub-7.2.0/pubnub/models/consumer/presence.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/pubsub.py` & `pubnub-7.2.0/pubnub/models/consumer/pubsub.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/push.py` & `pubnub-7.2.0/pubnub/models/consumer/push.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/time.py` & `pubnub-7.2.0/pubnub/models/consumer/time.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/access_manager.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/access_manager.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/channel.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/channel.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/group.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/group.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/pn_resource.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/pn_resource.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/space.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/space.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/user.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/user.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/consumer/v3/uuid.py` & `pubnub-7.2.0/pubnub/models/consumer/v3/uuid.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/models/server/subscribe.py` & `pubnub-7.2.0/pubnub/models/server/subscribe.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/pnconfiguration.py` & `pubnub-7.2.0/pubnub/pnconfiguration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from .enums import PNHeartbeatNotificationOptions, PNReconnectionPolicy
+from Cryptodome.Cipher import AES
+from pubnub.enums import PNHeartbeatNotificationOptions, PNReconnectionPolicy
+from pubnub.exceptions import PubNubException
 
 
 class PNConfiguration(object):
     DEFAULT_PRESENCE_TIMEOUT = 300
     DEFAULT_HEARTBEAT_INTERVAL = 280
+    ALLOWED_AES_MODES = [AES.MODE_CBC, AES.MODE_GCM]
 
     def __init__(self):
         # TODO: add validation
         self._uuid = None
         self.origin = "ps.pndsn.com"
         self.ssl = True
         self.non_subscribe_request_timeout = 10
         self.subscribe_request_timeout = 310
         self.connect_timeout = 10
         self.subscribe_key = None
         self.publish_key = None
         self.secret_key = None
         self.cipher_key = None
+        self._cipher_mode = AES.MODE_CBC
+        self._fallback_cipher_mode = None
         self.auth_key = None
         self.filter_expression = None
         self.enable_subscribe = True
         self.crypto_instance = None
         self.file_crypto_instance = None
         self.log_verbosity = False
         self.enable_presence_heartbeat = False
@@ -58,14 +63,38 @@
         self._presence_timeout = timeout
         self._heartbeat_interval = interval
 
     def set_presence_timeout(self, timeout):
         self.set_presence_timeout_with_custom_interval(timeout, (timeout / 2) - 1)
 
     @property
+    def cipher_mode(self):
+        return self._cipher_mode
+
+    @cipher_mode.setter
+    def cipher_mode(self, cipher_mode):
+        if cipher_mode not in self.ALLOWED_AES_MODES:
+            raise PubNubException('Cipher mode not supported')
+        if cipher_mode is not self._cipher_mode:
+            self._cipher_mode = cipher_mode
+            self.crypto_instance = None
+
+    @property
+    def fallback_cipher_mode(self):
+        return self._fallback_cipher_mode
+
+    @fallback_cipher_mode.setter
+    def fallback_cipher_mode(self, fallback_cipher_mode):
+        if fallback_cipher_mode not in self.ALLOWED_AES_MODES:
+            raise PubNubException('Cipher mode not supported')
+        if fallback_cipher_mode is not self._fallback_cipher_mode:
+            self._fallback_cipher_mode = fallback_cipher_mode
+            self.crypto_instance = None
+
+    @property
     def crypto(self):
         if self.crypto_instance is None:
             self._init_cryptodome()
 
         return self.crypto_instance
 
     def _init_cryptodome(self):
```

### Comparing `pubnub-7.1.0/pubnub/pubnub.py` & `pubnub-7.2.0/pubnub/pubnub.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/pubnub_asyncio.py` & `pubnub-7.2.0/pubnub/pubnub_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
         self._connector = None
         self._session = None
 
         self._connector = aiohttp.TCPConnector(verify_ssl=True)
         self._session = aiohttp.ClientSession(
             loop=self.event_loop,
-            conn_timeout=self.config.connect_timeout,
+            timeout=aiohttp.ClientTimeout(connect=self.config.connect_timeout),
             connector=self._connector
         )
 
         if self.config.enable_subscribe:
             self._subscription_manager = AsyncioSubscriptionManager(self)
 
         self._publish_sequence_manager = AsyncioPublishSequenceManager(self.event_loop, PubNubCore.MAX_SEQUENCE)
@@ -58,15 +58,15 @@
     async def set_connector(self, cn):
         await self._session.close()
 
         self._connector = cn
 
         self._session = aiohttp.ClientSession(
             loop=self.event_loop,
-            conn_timeout=self.config.connect_timeout,
+            timeout=aiohttp.ClientTimeout(connect=self.config.connect_timeout),
             connector=self._connector
         )
 
     async def stop(self):
         await self._session.close()
         if self._subscription_manager:
             self._subscription_manager.stop()
```

### Comparing `pubnub-7.1.0/pubnub/pubnub_core.py` & `pubnub-7.2.0/pubnub/pubnub_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 from .managers import TelemetryManager
 
 logger = logging.getLogger("pubnub")
 
 
 class PubNubCore:
     """A base class for PubNub Python API implementations"""
-    SDK_VERSION = "7.1.0"
+    SDK_VERSION = "7.2.0"
     SDK_NAME = "PubNub-Python"
 
     TIMESTAMP_DIVIDER = 1000
     MAX_SEQUENCE = 65535
 
     __metaclass__ = ABCMeta
     _plugins = []
```

### Comparing `pubnub-7.1.0/pubnub/request_handlers/requests_handler.py` & `pubnub-7.2.0/pubnub/request_handlers/requests_handler.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/structures.py` & `pubnub-7.2.0/pubnub/structures.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/utils.py` & `pubnub-7.2.0/pubnub/utils.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub/workers.py` & `pubnub-7.2.0/pubnub/workers.py`

 * *Files identical despite different names*

### Comparing `pubnub-7.1.0/pubnub.egg-info/PKG-INFO` & `pubnub-7.2.0/pubnub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pubnub
-Version: 7.1.0
+Version: 7.2.0
 Summary: PubNub Real-time push service in the cloud
 Home-page: http://pubnub.com
 Author: PubNub
 Author-email: support@pubnub.com
 License: MIT
 Project-URL: Source, https://github.com/pubnub/python
 Project-URL: Documentation, https://www.pubnub.com/docs/sdks/python
```

### Comparing `pubnub-7.1.0/pubnub.egg-info/SOURCES.txt` & `pubnub-7.2.0/pubnub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,20 @@
 pubnub/endpoints/pubsub/publish.py
 pubnub/endpoints/pubsub/subscribe.py
 pubnub/endpoints/push/__init__.py
 pubnub/endpoints/push/add_channels_to_push.py
 pubnub/endpoints/push/list_push_provisions.py
 pubnub/endpoints/push/remove_channels_from_push.py
 pubnub/endpoints/push/remove_device.py
+pubnub/event_engine/__init__.py
+pubnub/event_engine/dispatcher.py
+pubnub/event_engine/effects.py
+pubnub/event_engine/events.py
+pubnub/event_engine/statemachine.py
+pubnub/event_engine/states.py
 pubnub/models/__init__.py
 pubnub/models/subscription_item.py
 pubnub/models/consumer/__init__.py
 pubnub/models/consumer/access_manager.py
 pubnub/models/consumer/channel_group.py
 pubnub/models/consumer/common.py
 pubnub/models/consumer/file.py
```

### Comparing `pubnub-7.1.0/setup.py` & `pubnub-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pubnub',
-    version='7.1.0',
+    version='7.2.0',
     description='PubNub Real-time push service in the cloud',
     author='PubNub',
     author_email='support@pubnub.com',
     url='http://pubnub.com',
     project_urls={
         'Source': 'https://github.com/pubnub/python',
         'Documentation': 'https://www.pubnub.com/docs/sdks/python',
```

