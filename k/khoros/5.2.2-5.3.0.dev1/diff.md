# Comparing `tmp/khoros-5.2.2.tar.gz` & `tmp/khoros-5.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khoros-5.2.2.tar", last modified: Tue May 23 21:10:34 2023, max compression
+gzip compressed data, was "khoros-5.3.0.dev1.tar", last modified: Thu Jul  6 19:41:58 2023, max compression
```

## Comparing `khoros-5.2.2.tar` & `khoros-5.3.0.dev1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.582821 khoros-5.2.2/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.2.2/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)    17347 2023-05-23 21:10:34.582563 khoros-5.2.2/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.2.2/README.md
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.530787 khoros-5.2.2/khoros/
--rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    71382 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11278 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/auth.py
--rw-r--r--   0 shurtj     (501) staff       (20)    14393 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)   275817 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.537177 khoros-5.2.2/khoros/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.2.2/khoros/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11124 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.2.2/khoros/errors/translations.py
--rw-r--r--   0 shurtj     (501) staff       (20)    22871 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/liql.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.552338 khoros-5.2.2/khoros/objects/
--rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.2.2/khoros/objects/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.2.2/khoros/objects/albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/objects/archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.2.2/khoros/objects/attachments.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/objects/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)      519 2021-10-11 04:30:21.000000 khoros-5.2.2/khoros/objects/labels.py
--rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.2.2/khoros/objects/messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/objects/roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.2.2/khoros/objects/settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.2.2/khoros/objects/subscriptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/objects/tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/objects/users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/saml.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.559944 khoros-5.2.2/khoros/structures/
--rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.2.2/khoros/structures/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27629 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/boards.py
--rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.2.2/khoros/structures/categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/structures/grouphubs.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.2.2/khoros/structures/nodes.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.562274 khoros-5.2.2/khoros/studio/
--rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.2.2/khoros/studio/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2880 2020-10-30 02:28:27.000000 khoros-5.2.2/khoros/studio/base.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.566354 khoros-5.2.2/khoros/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.2.2/khoros/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/environment.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/log_utils.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.581698 khoros-5.2.2/khoros/utils/tests/
--rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.2.2/khoros/utils/tests/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/resources.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/test_archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_board_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/test_bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.2.2/khoros/utils/tests/test_categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.2.2/khoros/utils/tests/test_communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_error_handling.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.2.2/khoros/utils/tests/test_exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_grouphub_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_helper_file.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_http_headers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_library_import.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.2.2/khoros/utils/tests/test_liql.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_mentions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_node_id_extract.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.2.2/khoros/utils/tests/test_ssl_verify.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_studio.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.2.2/khoros/utils/tests/test_users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.2.2/khoros/utils/tests/test_version.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3786 2023-05-23 20:51:39.000000 khoros-5.2.2/khoros/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-05-23 21:10:34.533414 khoros-5.2.2/khoros.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)    17347 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-05-23 21:10:34.000000 khoros-5.2.2/khoros.egg-info/top_level.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      913 2023-05-23 20:51:39.000000 khoros-5.2.2/pyproject.toml
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-05-23 21:10:34.582898 khoros-5.2.2/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.2.2/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.652542 khoros-5.3.0.dev1/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.3.0.dev1/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-06 19:41:58.651457 khoros-5.3.0.dev1/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.3.0.dev1/README.md
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.580067 khoros-5.3.0.dev1/khoros/
+-rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    73826 2023-06-14 20:24:00.000000 khoros-5.3.0.dev1/khoros/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11891 2023-06-14 19:57:43.000000 khoros-5.3.0.dev1/khoros/auth.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    14989 2023-06-14 19:56:42.000000 khoros-5.3.0.dev1/khoros/bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)   278016 2023-06-06 21:08:56.000000 khoros-5.3.0.dev1/khoros/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.587945 khoros-5.3.0.dev1/khoros/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.3.0.dev1/khoros/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11117 2023-06-14 20:26:29.000000 khoros-5.3.0.dev1/khoros/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.3.0.dev1/khoros/errors/translations.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23051 2023-06-06 21:11:32.000000 khoros-5.3.0.dev1/khoros/liql.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.601598 khoros-5.3.0.dev1/khoros/objects/
+-rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.3.0.dev1/khoros/objects/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.3.0.dev1/khoros/objects/albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/objects/archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.3.0.dev1/khoros/objects/attachments.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/objects/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)      519 2021-10-11 04:30:21.000000 khoros-5.3.0.dev1/khoros/objects/labels.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.3.0.dev1/khoros/objects/messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/objects/roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.3.0.dev1/khoros/objects/settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.3.0.dev1/khoros/objects/subscriptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/objects/tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/objects/users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/saml.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.612649 khoros-5.3.0.dev1/khoros/structures/
+-rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/structures/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.3.0.dev1/khoros/structures/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    32351 2023-06-05 22:07:05.000000 khoros-5.3.0.dev1/khoros/structures/boards.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.3.0.dev1/khoros/structures/categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/structures/communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/structures/grouphubs.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.3.0.dev1/khoros/structures/nodes.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.615466 khoros-5.3.0.dev1/khoros/studio/
+-rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.3.0.dev1/khoros/studio/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2845 2023-06-14 20:27:59.000000 khoros-5.3.0.dev1/khoros/studio/base.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.622828 khoros-5.3.0.dev1/khoros/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.3.0.dev1/khoros/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/environment.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.650153 khoros-5.3.0.dev1/khoros/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.3.0.dev1/khoros/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_board_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_error_handling.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_grouphub_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_helper_file.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_http_headers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_library_import.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_liql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_mentions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_node_id_extract.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_ssl_verify.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_studio.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.3.0.dev1/khoros/utils/tests/test_version.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3790 2023-06-02 20:52:17.000000 khoros-5.3.0.dev1/khoros/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-06 19:41:58.583883 khoros-5.3.0.dev1/khoros.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-07-06 19:41:58.000000 khoros-5.3.0.dev1/khoros.egg-info/top_level.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      917 2023-06-20 13:43:52.000000 khoros-5.3.0.dev1/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-07-06 19:41:58.652755 khoros-5.3.0.dev1/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.3.0.dev1/setup.py
```

### Comparing `khoros-5.2.2/LICENSE` & `khoros-5.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/PKG-INFO` & `khoros-5.3.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.2.2
+Version: 5.3.0.dev1
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.2.2 Summary: Useful tools and
-utilities to assist in managing a Khoros Communities (formerly Lithium)
+Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev1 Summary: Useful tools
+and utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
```

### Comparing `khoros-5.2.2/README.md` & `khoros-5.3.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/__init__.py` & `khoros-5.3.0.dev1/khoros/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/api.py` & `khoros-5.3.0.dev1/khoros/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 :Module:            khoros.api
 :Synopsis:          This module handles interactions with the Khoros Community REST APIs
 :Usage:             ``import khoros.api``
 :Example:           ``json_response = khoros.api.get_request_with_retries(url, auth_dict=khoros.auth)``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     23 May 2022
+:Modified Date:     14 Jun 2023
 """
 
 import json
 import os.path
 import warnings
 import importlib
 
@@ -30,14 +30,17 @@
 ssl_warning_shown = False
 
 
 def define_headers(khoros_object=None, auth_dict=None, params=None, accept=None, content_type=None, multipart=False,
                    default_content_type=False, proxy_user_object=None):
     """This function defines the headers to use in an API call.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 4.0.0
        Introduced the ``proxy_user_object`` parameter to allow API requests to be performed on behalf of other users.
 
     .. versionchanged:: 3.5.0
        An unnecessary ``else`` statement after the :py:exc:`khoros.errors.exceptions.MissingAuthDataError`
        exception is raised has been removed.
 
@@ -57,26 +60,28 @@
     :type auth_dict: dict, None
     :param params: Header parameters in a dictionary format
     :type params: dict, None
     :param accept: The ``accept`` header value (e.g. ``application/json``)
     :type accept: str, None
     :param content_type: The ``content-type`` header value (e.g. ``application/json``)
     :type content_type: str, None
-    :param multipart: Defines whether or not the query is a ``multipart/form-data`` query (``False`` by default)
+    :param multipart: Defines whether the query is a ``multipart/form-data`` query (``False`` by default)
     :type multipart: bool
     :param default_content_type: Determines if ``application/json`` should be used as the default ``content-type``
                                  value if the key does not exist (``False`` by default)
     :type default_content_type: bool
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
     :returns: A dictionary with the header fields and associated values
     :raises: :py:exc:`khoros.errors.exceptions.MissingAuthDataError`
     """
     if not khoros_object and not auth_dict and not proxy_user_object:
+        error_msg = "The authentication data was not provided and a connection cannot be established."
+        logger.error(error_msg)
         raise errors.exceptions.MissingAuthDataError()
     if proxy_user_object:
         headers = proxy_user_object.session_header
     elif auth_dict:
         headers = auth_dict['header']
     else:
         headers = khoros_object.auth['header']
@@ -125,15 +130,15 @@
             _normalized_headers[_header_key] = _header_value
     return _normalized_headers
 
 
 def _get_json_query_string(_return_json, _include_ampersand_prefix=True):
     """This function constructs a query string for a Community API v1 query that should return JSON responses.
 
-    :param _return_json: Indicates whether or not API responses should be in JSON format
+    :param _return_json: Indicates whether API responses should be in JSON format
     :type _return_json: bool
     :param _include_ampersand_prefix: Determines if an ampersand (``&``) prefix should be included in the string
     :type _include_ampersand_prefix: bool
     :returns: The formatted query string
     """
     _query_strings = {True: 'restapi.response_format=json', False: ''}
     _prefixes = {True: '&', False: ''}
@@ -148,49 +153,53 @@
 
     .. versionadded:: 4.0.0
 
     .. note:: No action will be taken if the URI is not recognized as a Community API v1 URI.
 
     :param _uri: The current URI against which the REST API call will be made
     :type _uri: str
-    :param _return_json: Indicates whether or not the response should be in JSON format (``True`` by default)
+    :param _return_json: Indicates whether the response should be in JSON format (``True`` by default)
     :type _return_json: bool
     :returns: The URI either untouched or with the added query parameter string where appropriate
     :raises: :py:exc:`TypeError`
     """
     if 'restapi/vc' in _uri and 'restapi.response_format' not in _uri and _return_json:
         _has_queries = True if '?' in _uri else False
         _uri = f"{_uri}?" if '?' not in _uri else _uri
         _uri = f"{_uri}{_get_json_query_string(_return_json, _has_queries)}"
     return _uri
 
 
 def _display_ssl_verify_warning():
     """This function displays a warning if SSL verification has been disabled.
 
+    .. versionchanged:: 5.3.0
+       Added a warning log entry along with the warning message.
+
     .. versionchanged:: 5.0.0
        The redundant ``return`` statement has been removed.
 
     .. versionadded:: 4.3.0
 
     :returns: None
     """
     global ssl_warning_shown
     if ssl_warning_shown is False:
         # Warn that SSL warnings are being suppressed
-        warnings.warn('SSL certificate verification has been explicitly disabled and warnings '
-                      'will be suppressed')
+        _warn_msg = 'SSL certificate verification has been explicitly disabled and warnings will be suppressed'
+        logger.warn(_warn_msg)
+        warnings.warn(_warn_msg)
         ssl_warning_shown = True
 
         # Suppress warnings when performing API calls without verifying SSL certificates
         urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def should_verify_tls(khoros_object=None):
-    """This function determines whether or not to verify the server's TLS certificate. (``True`` by default)
+    """This function determines whether to verify the server's TLS certificate. (``True`` by default)
 
     .. versionchanged:: 4.3.0
        Introduced the ``ssl_verify_disabled`` global variable to allow this check to be performed even when the
        core object is not passed to the function.
 
     :param khoros_object: The core Khoros object
     :type khoros_object: class[khoros.Khoros], None
@@ -225,23 +234,23 @@
        value to prevent a linting error from being reported. Also leveraged the ``ssl_verify`` core setting.
 
     .. versionchanged:: 2.5.0
        Leverages new private functions and has improved error handling of JSON conversion attempts.
 
     :param query_url: The URI to be queried
     :type query_url: str
-    :param return_json: Determines whether or not the response should be returned in JSON format (Default: ``True``)
+    :param return_json: Determines whether the response should be returned in JSON format (Default: ``True``)
     :type return_json: bool
     :param khoros_object: The core Khoros object (Required if the ``auth_dict`` parameter is not supplied)
     :type khoros_object: class[khoros.Khoros], None
     :param auth_dict: The ``auth`` dictionary within the :py:class:`khoros.Khoros` class object
     :type auth_dict: dict, None
     :param headers: Any header values (in dictionary format) to pass in the API call (optional)
     :type headers: dict, None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
     :returns: The API response from the GET request (optionally in JSON format)
     :raises: :py:exc:`ValueError`, :py:exc:`TypeError`,
              :py:exc:`khoros.errors.exceptions.APIConnectionError`,
@@ -261,35 +270,38 @@
             retries += 1
     if retries == 6:
         _raise_exception_for_repeated_timeouts()
     return _attempt_json_conversion(response, return_json)
 
 
 def _is_plaintext_payload(_headers, _payload=None):
-    """This function checks to determine whether or not the payload for an API is in JSON or plaintext format.
+    """This function checks to determine whether the payload for an API is in JSON or plaintext format.
 
     .. versionadded:: 3.1.0
 
     :param _headers: The headers associated with the API call
     :type _headers: dict
     :param _payload: The payload to be delivered in the API call
     :type _payload: dict, str
-    :returns: Boolean value indicating whether or not the payload is plaintext
+    :returns: Boolean value indicating whether the payload is plaintext
     :raises: :py:exc:`ValueError`
     """
     _is_plaintext = False
     if ('content-type' in _headers and _headers.get('content-type') == 'text/plain') or isinstance(_payload, str):
         _is_plaintext = True
     return _is_plaintext
 
 
 def _api_request_with_payload(_url, _payload=None, _request_type='post', _headers=None, _multipart=False, _verify=None,
                               _khoros_object=None):
     """This function performs an API request while supplying a JSON payload.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 4.3.0
        An issue has been fixed that prevented SSL verification from being disabled by the helper file setting.
 
     .. versionchanged:: 3.5.0
        Removed the unnecessary ``pass`` statement.
 
     .. versionchanged:: 3.4.0
@@ -308,17 +320,17 @@
     :type _url: str
     :param _payload: The payload that accompanies the API call
     :type _payload: dict, str, None
     :param _request_type: Define the type of API call (e.g. ``get``, ``post`` or ``put``)
     :type _request_type: str
     :param _headers: Any predefined headers to be passed with the API call (optional)
     :type _headers: dict
-    :param _multipart: Defines whether or not the query is a ``multipart/form-data`` query (``False`` by default)
+    :param _multipart: Defines whether the query is a ``multipart/form-data`` query (``False`` by default)
     :type _multipart: bool
-    :param _verify: Determines whether or not to verify the server's TLS certificate (``None`` by default)
+    :param _verify: Determines whether to verify the server's TLS certificate (``None`` by default)
     :type _verify: bool
     :param _khoros_object: The core Khoros object
     :type _khoros_object: class[khoros.Khoros], None
     :returns: The API response
     :raises: :py:exc:`khoros.errors.exceptions.InvalidRequestTypeError`,
              :py:exc:`khoros.errors.exceptions.APIConnectionError`
     """
@@ -340,40 +352,45 @@
                 elif _request_type.lower() == "post":
                     if _multipart:
                         _response = requests.post(_url, files=_payload, headers=_headers, verify=_verify)
                     else:
                         _payload = json.dumps(_payload, default=str) if not _is_plaintext else _payload
                         _response = requests.post(_url, data=_payload, headers=_headers, verify=_verify)
                 else:
+                    _error_msg = 'The supplied request type for the API is not recognized.'
+                    logger.error(_error_msg)
                     raise errors.exceptions.InvalidRequestTypeError()
                 break
             except Exception as _exc_msg:
                 _report_failed_attempt(_exc_msg, _request_type, _retries)
                 _retries += 1
         if _retries == 6:
             _raise_exception_for_repeated_timeouts()
     return _response
 
 
 def _api_request_without_payload(_url, _request_type, _headers, _verify=None, _khoros_object=None):
     """This function performs a ``POST`` or ``PUT`` request without an accompanying JSON payload.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 4.3.0
        An issue has been fixed that prevented SSL verification from being disabled by the helper file setting.
 
     .. versionchanged:: 3.4.0
        Support has been introduced for the ``_verify`` parameter to determine if SSL certificate verification is needed.
 
     :param _url: The URL for the API request
     :type _url: str
     :param _request_type: The request type (e.g. ``post`` or ``put``)
     :type _request_type: str
     :param _headers: The headers associated with the API request
     :type _headers: dict
-    :param _verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param _verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type _verify: bool
     :param _khoros_object: The core Khoros object
     :type _khoros_object: class[khoros.Khoros], None
     :returns: The API response
     :raises: :py:exc:`khoros.errors.exceptions.InvalidRequestTypeError`,
              :py:exc:`khoros.errors.exceptions.APIConnectionError`
     """
@@ -382,14 +399,16 @@
     while _retries <= 5:
         try:
             if _request_type.lower() == "post":
                 _response = requests.post(_url, headers=_headers, verify=_verify)
             elif _request_type.lower() == "put":
                 _response = requests.put(_url, headers=_headers, verify=_verify)
             else:
+                _error_msg = 'The supplied request type for the API is not recognized.'
+                logger.error(_error_msg)
                 raise errors.exceptions.InvalidRequestTypeError()
             break
         except Exception as _exc_msg:
             _report_failed_attempt(_exc_msg, _request_type, _retries)
             _retries += 1
     if _retries == 6:
         _raise_exception_for_repeated_timeouts()
@@ -426,49 +445,62 @@
     """
     return {'avatar': (f'{os.path.basename(avatar_image_path)}', open(avatar_image_path, 'rb'))}
 
 
 def _report_failed_attempt(_exc_msg, _request_type, _retries):
     """This function reports a failed API call that will be retried.
 
+    .. versionchanged:: 5.3.0
+       Added error logging and changed the generic exception to a :py:exc:`RuntimeError` exception.
+
     .. versionchanged:: 5.0.0
        The redundant ``return`` statement has been removed.
 
-    :param _exc_msg: The exception that was raised can captured within a try/except clause
+    :param _exc_msg: The exception that was raised and captured within a try/except clause
     :param _request_type: The type of API request (e.g. ``post``, ``put`` or ``get``)
     :type _request_type: str
     :param _retries: The attempt number for the API request
     :type _retries: int
     :returns: None
     """
     _exc_name = type(_exc_msg).__name__
     if 'connect' not in _exc_name.lower():
-        raise Exception(f"{_exc_name}: {_exc_msg}")
+        _error_msg = f"{_exc_name}: {_exc_msg}"
+        logger.error(_error_msg)
+        raise RuntimeError(_error_msg)
     _current_attempt = f"(Attempt {_retries} of 5)"
     _error_msg = f"The {_request_type.upper()} request has failed with the following exception: " + \
                  f"{_exc_name}: {_exc_msg} {_current_attempt}"
+    logger.error(_error_msg)
     errors.handlers.eprint(f"{_error_msg}\n{_exc_name}: {_exc_msg}\n")
 
 
 def _raise_exception_for_repeated_timeouts():
     """This function raises an exception when all API attempts (including) retries resulted in a timeout.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     :returns: None
     :raises: :py:exc:`khoros.errors.exceptions.APIConnectionError`
     """
     _failure_msg = "The script was unable to complete successfully after five consecutive API timeouts. " + \
                    "Please run the script again or contact Khoros Support for further assistance."
+    logger.error(_failure_msg)
     raise errors.exceptions.APIConnectionError(_failure_msg)
 
 
 def payload_request_with_retries(url, request_type, json_payload=None, plaintext_payload=None, url_encoded_payload=None,
                                  return_json=True, khoros_object=None, auth_dict=None, headers=None, multipart=False,
                                  content_type=None, verify=None, proxy_user_object=None):
     """This function performs an API request that includes a payload with up to three reties as necessary.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 4.0.0
        Introduced the ``proxy_user_object`` parameter to allow API requests to be performed on behalf of other users.
 
     .. versionchanged:: 3.4.0
        Support has been introduced for the ``ssl_verify`` core setting in the :py:class:`khoros.core.Khoros` object.
 
     .. versionchanged:: 3.2.0
@@ -480,31 +512,31 @@
     :type request_type: str
     :param json_payload: The payload for the POST or PUT request in JSON format
     :type json_payload: dict, None
     :param plaintext_payload: The payload for the POST or PUT request in plaintext (i.e. ``text/plain``) format
     :type plaintext_payload: str, None
     :param url_encoded_payload: The payload for the POST or PUT request as a URL-encoded string
     :type url_encoded_payload: str, None
-    :param return_json: Determines whether or not the response should be returned in JSON format (Default: ``True``)
+    :param return_json: Determines whether the response should be returned in JSON format (Default: ``True``)
     :type return_json: bool
     :param khoros_object: The core Khoros object (Required if the ``auth_dict`` parameter is not supplied)
     :type khoros_object: class[khoros.Khoros], None
     :param auth_dict: The ``auth`` dictionary within the :py:class:`khoros.Khoros` class object
     :type auth_dict: dict, None
     :param headers: Any header values (in dictionary format) to pass in the API call (optional)
     :type headers: dict, None
-    :param multipart: Defines whether or not the query is a ``multipart/form-data`` query (``False`` by default)
+    :param multipart: Defines whether the query is a ``multipart/form-data`` query (``False`` by default)
     :type multipart: bool
     :param content_type: Allows the ``content-type`` value to be explicitly defined if necessary
 
                          .. note:: If this parameter is not defined then the content type will be identified based
                                    on the payload format and/or type of request.
 
     :type content_type: str, None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
     :returns: The API response from the API request
     :raises: :py:exc:`ValueError`, :py:exc:`khoros.errors.exceptions.APIConnectionError`,
              :py:exc:`khoros.errors.exceptions.POSTRequestError`,
@@ -512,14 +544,16 @@
              :py:exc:`khoros.errors.exceptions.InvalidRequestTypeError`,
              :py:exc:`khoros.errors.exceptions.PayloadMismatchError`
     """
     # Ensure that the request type is valid
     valid_request_types = ['post', 'put']
     request_type = request_type.lower()
     if request_type not in valid_request_types:
+        error_msg = 'The supplied request type for the API is not recognized.'
+        logger.error(error_msg)
         raise errors.exceptions.InvalidRequestTypeError()
 
     # Determine if TLS certificates should be verified during API calls
     verify = should_verify_tls(khoros_object) if verify is None else verify
 
     # Construct the appropriate headers for the POST call
     if content_type:
@@ -537,18 +571,22 @@
     if any((plaintext_payload, url_encoded_payload, json_payload)):
         if any((plaintext_payload, url_encoded_payload)) and not json_payload:
             if plaintext_payload and not url_encoded_payload:
                 payload = plaintext_payload
             elif url_encoded_payload and not plaintext_payload:
                 payload = url_encoded_payload
             else:
+                error_msg = 'More than one payload was provided for the API call when only one is permitted.'
+                logger.error(error_msg)
                 raise errors.exceptions.PayloadMismatchError(request_type=request_type.upper())
         elif json_payload and not any((plaintext_payload, url_encoded_payload)):
             payload = json_payload
         else:
+            error_msg = 'More than one payload was provided for the API call when only one is permitted.'
+            logger.error(error_msg)
             raise errors.exceptions.PayloadMismatchError(request_type=request_type.upper())
     else:
         payload = None
     response = _api_request_with_payload(url, payload, request_type, headers, multipart, verify)
     return _attempt_json_conversion(response, return_json)
 
 
@@ -585,31 +623,31 @@
     :type url: str
     :param json_payload: The payload for the POST request in JSON format
     :type json_payload: dict, None
     :param plaintext_payload: The payload for the POST request in plaintext (i.e. ``text/plain``) format
     :type plaintext_payload: str, None
     :param url_encoded_payload: The payload for the POST request as a URL-encoded string
     :type url_encoded_payload: str, None
-    :param return_json: Determines whether or not the response should be returned in JSON format (Default: ``True``)
+    :param return_json: Determines whether the response should be returned in JSON format (Default: ``True``)
     :type return_json: bool
     :param khoros_object: The core Khoros object (Required if the ``auth_dict`` parameter is not supplied)
     :type khoros_object: class[khoros.Khoros], None
     :param auth_dict: The ``auth`` dictionary within the :py:class:`khoros.Khoros` class object
     :type auth_dict: dict, None
     :param headers: Any header values (in dictionary format) to pass in the API call (optional)
     :type headers: dict, None
-    :param multipart: Defines whether or not the query is a ``multipart/form-data`` query (``False`` by default)
+    :param multipart: Defines whether the query is a ``multipart/form-data`` query (``False`` by default)
     :type multipart: bool
     :param content_type: Allows the ``content-type`` value to be explicitly defined if necessary
 
                          .. note:: If this parameter is not defined then the content type will be identified based
                                    on the payload format and/or type of request.
 
     :type content_type: str, None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
     :returns: The API response from the POST request
     :raises: :py:exc:`ValueError`, :py:exc:`khoros.errors.exceptions.APIConnectionError`,
              :py:exc:`khoros.errors.exceptions.POSTRequestError`,
@@ -663,31 +701,31 @@
     :type url: str
     :param json_payload: The payload for the PUT request in JSON format
     :type json_payload: dict, None
     :param plaintext_payload: The payload for the POST request in plaintext (i.e. ``text/plain``) format
     :type plaintext_payload: str, None
     :param url_encoded_payload: The payload for the POST request as a URL-encoded string
     :type url_encoded_payload: str, None
-    :param return_json: Determines whether or not the response should be returned in JSON format (Default: ``True``)
+    :param return_json: Determines whether the response should be returned in JSON format (Default: ``True``)
     :type return_json: bool
     :param khoros_object: The core Khoros object (Required if the ``auth_dict`` parameter is not supplied)
     :type khoros_object: class[khoros.Khoros], None
     :param auth_dict: The ``auth`` dictionary within the :py:class:`khoros.Khoros` class object
     :type auth_dict: dict, None
     :param headers: Any header values (in dictionary format) to pass in the API call (optional)
     :type headers: dict, None
-    :param multipart: Defines whether or not the query is a ``multipart/form-data`` query (``False`` by default)
+    :param multipart: Defines whether the query is a ``multipart/form-data`` query (``False`` by default)
     :type multipart: bool
     :param content_type: Allows the ``content-type`` value to be explicitly defined if necessary
 
                          .. note:: If this parameter is not defined then the content type will be identified based
                                    on the payload format and/or type of request.
 
     :type content_type: str, None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
     :returns: The API response from the PUT request
     :raises: :py:exc:`ValueError`, :py:exc:`khoros.errors.exceptions.APIConnectionError`,
              :py:exc:`khoros.errors.exceptions.PUTRequestError`,
@@ -701,36 +739,41 @@
                                         multipart=multipart, content_type=content_type.lower(), verify=verify,
                                         proxy_user_object=proxy_user_object)
 
 
 def _attempt_json_conversion(_response, _return_json):
     """This function attempts to convert an API response to JSON if requested.
 
+    .. versionchanged:: 5.3.0
+       Added an error log entry for the error before it is printed onscreen.
+
     .. versionadded:: 2.5.0
 
     :param _response: The API response to be converted
-    :param _return_json: Indicates whether or not the API response should be converted
+    :param _return_json: Indicates whether the API response should be converted
     :type _return_json: bool
     :returns: The API response that has been converted to JSON or in its original format if unable to convert
     """
     if _return_json and not isinstance(_response, dict):
         try:
             _response = _response.json()
         except Exception as _exc_msg:
             _exc_name = type(_exc_msg).__name__
-            errors.handlers.eprint(f"Failed to convert to JSON due to the following exception: {_exc_name}: {_exc_msg}")
+            _error_msg = f"Failed to convert to JSON due to the following exception: {_exc_name}: {_exc_msg}"
+            logger.error(_error_msg)
+            errors.handlers.eprint(_error_msg)
     return _response
 
 
 def query_successful(api_response):
-    """This function reviews the API response from the Community API to verify whether or not the call was successful.
+    """This function reviews the API response from the Community API to verify whether the call was successful.
 
     :param api_response: The response from the API in JSON format
     :type api_response: dict
-    :returns: Boolean indicating whether or not the API call was successful
+    :returns: Boolean indicating whether the API call was successful
     """
     try:
         success_values = ['successful', 'success']
         successful = True if api_response['status'] in success_values else False
     except (KeyError, IndexError, ValueError, TypeError):
         successful = False
     return successful
@@ -767,26 +810,26 @@
        Introduced the ``proxy_user_object`` parameter to allow API requests to be performed on behalf of other users.
 
     .. versionchanged:: 3.4.0
        Support has been introduced for the ``ssl_verify`` core setting in the :py:class:`khoros.core.Khoros` object.
 
     :param url: The URI against which the DELETE request will be issued
     :type url: str
-    :param return_json: Determines whether or not the response should be returned in JSON format (Default: ``False``)
+    :param return_json: Determines whether the response should be returned in JSON format (Default: ``False``)
     :type return_json: bool
     :param khoros_object: The core Khoros object (Required if the ``auth_dict`` parameter is not supplied)
     :type khoros_object: class[khoros.Khoros], None
     :param auth_dict: The ``auth`` dictionary within the :py:class:`khoros.Khoros` class object
     :type auth_dict: dict, None
     :param headers: Any header values (in dictionary format) to pass in the API call (optional)
     :type headers: dict, None
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :returns: The API response from the DELETE request (optionally in JSON format)
     """
     # Determine if TLS certificates should be verified during API calls
     verify = should_verify_tls(khoros_object) if verify is None else verify
 
     # Perform the API call to delete the asset
@@ -797,14 +840,17 @@
         response = response.json()
     return response
 
 
 def get_v1_node_collection(node_type):
     """This function retrieves the appropriate API v1 collection name for a given node type.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 4.0.0
        Group Hubs are now supported by the function by passing the ``grouphub`` or ``group hub`` string.
 
     .. versionadded:: 3.5.0
 
     :param node_type: The node type for which to retrieve the collection (e.g. ``board``, ``category``)
     :type node_type: str
@@ -815,22 +861,27 @@
         'board': 'boards',
         'category': 'categories',
         'grouphub': 'nodes/type/key/grouphub',
         'group hub': 'nodes/type/key/grouphub',
     }
     node_collection = node_type if node_type in node_collections.values() else ''
     if node_type not in node_collections:
+        error_msg = 'The node type that was provided is invalid.'
+        logger.error(error_msg)
         raise errors.exceptions.InvalidNodeTypeError(val=node_type)
     return node_collections.get(node_type) if not node_collection else node_collection
 
 
 def get_v1_user_path(user_id=None, user_email=None, user_login=None, user_sso_id=None, user_and_type=None,
                      trailing_slash=False):
     """This function returns the segment of an API v1 endpoint that is the path to define a user.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionadded:: 4.0.0
        Introduced the ``user_and_type`` parameter that can be passed instead of a parameter for a specific type.
 
     .. versionadded:: 3.5.0
 
     :param user_id: The numeric User ID associated with a user
     :type user_id: str, int, None
@@ -852,15 +903,17 @@
     user_id = user_and_type[0] if user_and_type[1] == 'id' else user_id
     user_email = user_and_type[0] if user_and_type[1] == 'email' else user_email
     user_login = user_and_type[0] if user_and_type[1] == 'login' else user_login
     user_sso_id = user_and_type[0] if user_and_type[1] == 'sso_id' else user_sso_id
 
     # Validate the data and return the path
     if not any((user_id, user_email, user_login, user_sso_id)):
-        raise errors.exceptions.MissingRequiredDataError("A user identifier must be provided")
+        error_msg = "A user identifier must be provided"
+        logger.error(error_msg)
+        raise errors.exceptions.MissingRequiredDataError(error_msg)
     slash = '/' if trailing_slash else ''
     if user_email:
         user_path = f"/users/email/{user_email}{slash}"
     elif user_login:
         user_path = f"/users/login/{user_login}{slash}"
     elif user_sso_id:
         user_path = f"/users/sso_id/{user_sso_id}{slash}"
@@ -896,15 +949,15 @@
     :param return_json: Determines if the response should be returned in JSON format (``False`` by default)
     :type return_json: bool
     :param fail_on_no_results: Raises an exception if no results are returned (``False`` by default)
     :type fail_on_no_results: bool
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :returns: The API response (optionally in JSON format)
     :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
     """
     # Determine if TLS certificates should be verified during API calls
     verify = should_verify_tls(khoros_object) if verify is None else verify
 
@@ -990,14 +1043,17 @@
     return core_utils.encode_query_string(query_dict, json_payload=json_payload)
 
 
 def make_v1_request(khoros_object, endpoint, query_params=None, request_type='GET', return_json=True,
                     params_in_uri=False, json_payload=False, proxy_user_object=None, verify=None):
     """This function makes a Community API v1 request.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 4.3.0
        An issue has been fixed that prevented SSL verification from being disabled by the helper file setting.
 
     .. versionchanged:: 4.0.0
        Introduced the ``proxy_user_object`` parameter to allow API requests to be performed on behalf of other users.
 
     .. versionchanged:: 3.2.0
@@ -1037,15 +1093,15 @@
 
                          .. caution:: This is not yet fully supported and therefore should not be used at this time.
 
     :type json_payload: bool
     :param proxy_user_object: Instantiated :py:class:`khoros.objects.users.ImpersonatedUser` object to perform the
                               API request on behalf of a secondary user.
     :type proxy_user_object: class[khoros.objects.users.ImpersonatedUser], None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :returns: The API response
     :raises: :py:exc:`ValueError`, :py:exc:`TypeError`,
              :py:exc:`khoros.errors.exceptions.GETRequestError`,
              :py:exc:`khoros.errors.exceptions.POSTRequestError`,
              :py:exc:`khoros.errors.exceptions.PUTRequestError`,
              :py:exc:`khoros.errors.exceptions.APIConnectionError`,
@@ -1103,17 +1159,21 @@
                                                 proxy_user_object=proxy_user_object, verify=verify)
         else:
             response = put_request_with_retries(url, url_encoded_payload=query_string, return_json=return_json,
                                                 khoros_object=khoros_object, headers=header,
                                                 proxy_user_object=proxy_user_object, verify=verify)
     elif request_type.upper() in currently_unsupported_types:
         # TODO: Pass the request type into the exception to provide a more specific error
+        error_msg = 'This feature is currently unsupported at this time.'
+        logger.error(error_msg)
         raise errors.exceptions.CurrentlyUnsupportedError()
     else:
         # TODO: Pass the request type into the exception to provide a more specific error
+        error_msg = 'This feature is currently unsupported at this time.'
+        logger.error(error_msg)
         raise errors.exceptions.InvalidRequestTypeError()
     return response
 
 
 def deliver_v2_results(response, full_response=None, return_id=None, return_url=None, return_api_url=None,
                        return_http_code=None, return_status=None, return_error_messages=None, split_errors=False,
                        khoros_object=None):
@@ -1145,15 +1205,15 @@
     :param return_error_messages: Determines if error messages should be returned when applicable
     :type return_error_messages: bool, None
     :param split_errors: Determines if error messages should be split into separate values or merged when applicable
     :type split_errors: bool
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros], None
 
-                         .. note:: The core object is only leveraged to check whether or not the ``translate_errors``
+                         .. note:: The core object is only leveraged to check whether the ``translate_errors``
                                    setting is configured and to retrieve its value where possible.
 
     :returns: Boolean value indicating a successful outcome (default), the full API response or one or more specific
               fields defined by function arguments
     """
     outcome = query_successful(response)
     if any((return_id, return_url, return_api_url, return_http_code, return_status, return_error_messages)):
@@ -1216,15 +1276,15 @@
     :param data_api_uri: Defines if the **API URI** should be returned
     :type data_api_uri: bool
     :param v2_base: The base URL for the API v2
     :type v2_base: str, None
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros], None
 
-                         .. note:: The core object is only leveraged to check whether or not the ``translate_errors``
+                         .. note:: The core object is only leveraged to check whether the ``translate_errors``
                                    setting is configured and to retrieve its value where possible.
 
     :returns: A string, tuple or dictionary with the parsed data
     :raises: :py:exc:`khoros.errors.exceptions.MissingRequiredDataError`
     """
     parsed_data = {}
     dev_msg = True if error_msg or dev_msg else False
@@ -1280,20 +1340,20 @@
 
     .. versionadded:: 2.5.2
 
     :param _return_booleans: Dictionary of the return types with their associated Boolean value
     :type _return_booleans: dict
     :param _api_response: The Khoros Community API v2 response
     :type _api_response: dict
-    :param _split_errors: Defines whether or not error messages should be merged when applicable
+    :param _split_errors: Defines whether error messages should be merged when applicable
     :type _split_errors: bool
     :param _khoros_object: The core :py:class:`khoros.Khoros` object
     :type _khoros_object: class[khoros.Khoros], None
 
-                          .. note:: The core object is only leveraged to check whether or not the ``translate_errors``
+                          .. note:: The core object is only leveraged to check whether the ``translate_errors``
                                     setting is configured and to retrieve its value where possible.
 
     :returns: A dictionary of the parsed return values for return types whose Boolean values are ``True``
     """
     _return_values = {}
     for _return_type, _return_boolean in _return_booleans.items():
         if _return_boolean:
@@ -1321,14 +1381,17 @@
                 pass
     return _return_values
 
 
 def _confirm_field_supplied(_fields_dict):
     """This function checks to ensure that at least one field has been enabled to retrieve.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 5.0.0
        The redundant ``return`` statement has been removed.
 
     .. versionchanged:: 2.5.0
        Moved from the :py:mod:`khoros.objects.messages` module to :py:mod:`khoros.api`.
 
     .. versionadded:: 2.3.0
@@ -1340,15 +1403,17 @@
     """
     _field_supplied = False
     for _field_value in _fields_dict.values():
         if _field_value[0]:
             _field_supplied = True
             break
     if not _field_supplied:
-        raise errors.exceptions.MissingRequiredDataError("At least one field must be enabled to retrieve a response.")
+        _error_msg = "At least one field must be enabled to retrieve a response."
+        logger.error(_error_msg)
+        raise errors.exceptions.MissingRequiredDataError(_error_msg)
 
 
 def _normalize_base_url(_base_url):
     """This function normalizes the base URL (i.e. top-level domain) for use in other functions.
 
     .. versionadded:: 3.0.0
 
@@ -1385,15 +1450,15 @@
     :type simple: bool
     :param commit_id: Defines if the Commit ID (i.e. hash) for the release should be returned
     :type commit_id: bool
     :param timestamp: Defines if the timestamp of the release (e.g. 2007092156) should be returned
     :type timestamp: bool
     :param khoros_object: The core Khoros object (Optional unless needing to determine SSL certificate verification)
     :type khoros_object: class[khoros.Khoros], None
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :returns: One or more string with version information
     :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
     """
     # Determine if TLS certificates should be verified during API calls
     verify = should_verify_tls(khoros_object) if verify is None else verify
```

### Comparing `khoros-5.2.2/khoros/auth.py` & `khoros-5.3.0.dev1/khoros/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 :Module:            khoros.auth
 :Synopsis:          This module handles authentication-related tasks and operations for the Khoros Community APIs
 :Usage:             ``import khoros.auth``
 :Example:           ``session_key = khoros.auth(KhorosObject)``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     23 May 2022
+:Modified Date:     14 Jun 2023
 """
 
 import requests
 from defusedxml import ElementTree
 
 from . import api, errors
 from .utils import core_utils, log_utils
@@ -18,14 +18,17 @@
 # Initialize the logger for this module
 logger = log_utils.initialize_logging(__name__)
 
 
 def get_session_key(khoros_object, username=None, password=None):
     """This function retrieves the session key for an authentication session.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 5.0.0
        The error handling has been improved to provide more useful information when applicable.
 
     .. versionchanged:: 4.2.0
        The URI is now generated utilizing the :py:func:`khoros.auth._get_khoros_login_url` function.
 
     .. versionchanged:: 3.5.0
@@ -63,36 +66,45 @@
     secondary_user = False if password else True
     header = _get_session_key_header(khoros_object, secondary_user)
     response = requests.post(uri, headers=header, verify=verify)
     if response.status_code != 200:
         if type(response.text) == str and response.text.startswith('<html>'):
             api_error = errors.handlers.get_error_from_html(response.text)
             error_msg = f"The authentication attempt failed with the following error:\n\t{api_error}"
+            logger.error(error_msg)
             raise errors.exceptions.SessionAuthenticationError(error_msg)
         raise errors.exceptions.SessionAuthenticationError()
     else:
         response = response.json()
         if isinstance(response, dict) and 'response' in response and response['response'].get('status') == 'error':
             try:
                 error_msg = response['response']['error']['message']
                 full_error_msg = f"Session key authentication failed for '{username}': {error_msg}"
+                logger.error(full_error_msg)
                 raise errors.exceptions.SessionAuthenticationError(full_error_msg)
             except KeyError:
-                raise errors.exceptions.SessionAuthenticationError(f"Failed to retrieve a session key for '{username}'")
+                error_msg = f"Failed to retrieve a session key for '{username}'"
+                logger.error(error_msg)
+                raise errors.exceptions.SessionAuthenticationError(error_msg)
         else:
             try:
                 session_key = response['response']['value']['$']
             except KeyError:
-                raise errors.exceptions.SessionAuthenticationError(f"Failed to retrieve a session key for '{username}'")
+                error_msg = f"Failed to retrieve a session key for '{username}'"
+                logger.error(error_msg)
+                raise errors.exceptions.SessionAuthenticationError(error_msg)
     return session_key
 
 
 def get_sso_key(khoros_object):
     """This function retrieves the session key for a LithiumSSO session.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 5.0.0
        The two ``if`` statements have been merged.
 
     .. versionadded:: 4.2.0
 
     :param khoros_object: The core Khoros object
     :type khoros_object: class[khoros.Khoros]
@@ -106,15 +118,17 @@
         khoros_login_url,
         headers=headers,
         data=khoros_object.core_settings.get('sso')
     )
     tree = ElementTree.fromstring(response.text)
     if 'status' in tree.attrib and tree.attrib['status'] == 'success':
         return tree.findtext('value')
-    raise errors.exceptions.SsoAuthenticationError('Failed to retrieve a session key with the LithiumSSO token.')
+    error_msg = 'Failed to retrieve a session key with the LithiumSSO token.'
+    logger.error(error_msg)
+    raise errors.exceptions.SsoAuthenticationError(error_msg)
 
 
 def _get_khoros_login_url(khoros_object):
     """This function returns the URL for the Khoros login endpoint.
 
     .. versionadded:: 4.2.0
 
@@ -150,28 +164,32 @@
         _auth_payload.update({'restapi.response_format': 'json'})
     return _auth_payload
 
 
 def _get_session_key_header(_khoros_object, _secondary=False):
     """This function retrieves the header for an API call to retrieve a session key.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionadded:: 3.5.0
 
     :param _khoros_object: The core Khoros object
     :type _khoros_object: class[khoros.Khoros]
     :param _secondary: Indicates that the authentication request is for a secondary user (``False`` by default)
     :returns: A dictionary with the header information
     :raises: :py:exc:`khoros.errors.exceptions.SessionAuthenticationError`
     """
     _header = {"content-type": "application/x-www-form-urlencoded"}
     if _secondary:
         if _khoros_object.auth.get('header'):
             _header.update(_khoros_object.auth.get('header'))
         else:
             _error_msg = "Unable to retrieve a session key for secondary users without an existing session key"
+            logger.error(_error_msg)
             raise errors.exceptions.SessionAuthenticationError(_error_msg)
     return _header
 
 
 def get_session_header(session_key):
     """This function constructs and returns a proper API header containing the session key for authorization.
```

### Comparing `khoros-5.2.2/khoros/bulk_data.py` & `khoros-5.3.0.dev1/khoros/bulk_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 :Module:            khoros.objects.bulk_data
 :Synopsis:          This module includes functions that relate to the Bulk Data API.
 :Usage:             ``from khoros import bulk_data``
 :Example:           ``base_url = bulk_data.get_base_url(community_id='example.prod')``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     01 Nov 2022
+:Modified Date:     14 Jun 2023
 """
 
 import requests
 
 from . import errors
 from .utils import log_utils
 
@@ -60,14 +60,17 @@
     return base_url
 
 
 def query(khoros_object=None, community_id=None, client_id=None, token=None, from_date=None, to_date=None, fields=None,
           europe=None, export_type=None, full_response=False):
     """This function performs a query against the Bulk Data API to retrieve CSV or JSON data.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionchanged:: 5.2.0
        Improved the error handling to display the response text in the raised exception when available.
 
     .. versionadded:: 5.0.0
 
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros], None
@@ -101,23 +104,26 @@
         base_url = get_base_url(khoros_object, community_id, europe)
 
     # Get the client ID
     if not client_id:
         if khoros_object and khoros_object.bulk_data_settings.get('client_id'):
             client_id = khoros_object.bulk_data_settings.get('client_id')
         else:
-            raise errors.exceptions.MissingAuthDataError('A valid Client ID is required to utilize the Bulk Data API.')
+            error_msg = 'A valid Client ID is required to utilize the Bulk Data API.'
+            logger.error(error_msg)
+            raise errors.exceptions.MissingAuthDataError(error_msg)
 
     # Get the auth token
     if not token:
         if khoros_object and khoros_object.bulk_data_settings.get('token'):
             token = khoros_object.bulk_data_settings.get('token')
         else:
-            raise errors.exceptions.MissingAuthDataError('A valid access token is required to utilize the '
-                                                         'Bulk Data API.')
+            error_msg = 'A valid access token is required to utilize the Bulk Data API.'
+            logger.error(error_msg)
+            raise errors.exceptions.MissingAuthDataError(error_msg)
 
     # Construct the API headers
     headers = _construct_headers(khoros_object, client_id, export_type)
 
     # Construct the authentication tuple
     auth = (token, '')
 
@@ -127,14 +133,15 @@
     # Perform the API call
     response = requests.get(base_url, params=params, auth=auth, headers=headers)
     if not full_response:
         if response.status_code != 200:
             exc_msg = f'Bulk Data API request failed with a {response.status_code} response.'
             if response.text:
                 exc_msg = exc_msg.replace('.', f': {response.text}')
+            logger.error(exc_msg)
             raise errors.exceptions.APIRequestError(exc_msg)
         if export_type.lower() == 'json':
             response = response.json()
         else:
             response = response.text
     return response
 
@@ -159,14 +166,17 @@
     filtered_data = {'records': filtered_data}
     return filtered_data
 
 
 def filter_anonymous(bulk_data, remove_anonymous=None, remove_registered=None):
     """This function filters bulk data entries to keep only registered (default) or anonymous user activities.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionadded:: 5.2.0
 
     :param bulk_data: The Bulk Data API export in JSON format (i.e. dictionary)
     :type bulk_data: dict
     :param remove_anonymous: Determines if all anonymous user activities should be removed (Default)
     :type remove_anonymous: bool, None
     :param remove_registered: Determines if all registered user activities should be removed
@@ -176,17 +186,21 @@
              :py:exc:`khoros.errors.exceptions.InvalidParameterError`
     """
     filtered_data = []
     _validate_bulk_data_export(bulk_data)
     if remove_anonymous is None and remove_registered is None:
         remove_anonymous = True
     if remove_anonymous and remove_registered:
-        raise errors.exceptions.InvalidParameterError('You cannot remove both anonymous and registered users.')
+        error_msg = 'You cannot remove both anonymous and registered users.'
+        logger.error(error_msg)
+        raise errors.exceptions.InvalidParameterError(error_msg)
     if not remove_anonymous and not remove_registered:
-        raise errors.exceptions.InvalidParameterError('You must remove either anonymous or registered users.')
+        error_msg = 'You must remove either anonymous or registered users.'
+        logger.error(error_msg)
+        raise errors.exceptions.InvalidParameterError(error_msg)
     for entry in bulk_data['records']:
         if (remove_anonymous and entry.get('user.registration_status') != 'ANONYMOUS') or \
                 (remove_registered and entry.get('user.registration_status') == 'ANONYMOUS'):
             filtered_data.append(entry)
     filtered_data = {'records': filtered_data}
     return filtered_data
 
@@ -296,14 +310,17 @@
             (len(_date_value) != 8 and len(_date_value) != 12):
         raise ValueError('The fromDate and toDate fields should be in yyyyMMdd or yyyyMMddHHmm format.')
 
 
 def _construct_headers(_khoros_object=None, _client_id=None, _export_type=None):
     """This function constructs the headers to use in a Bulk Data API call.
 
+    .. versionchanged:: 5.3.0
+       Added logging error messages when exceptions are raised.
+
     .. versionadded:: 5.0.0
 
     :param _khoros_object: The core :py:class:`khoros.Khoros` object
     :type _khoros_object: class[khoros.Khoros], None
     :param _client_id: The Client ID to use when authenticating the API calls
     :type _client_id: str, None
     :param _export_type: Indicates the export type as either ``csv`` (default) or ``json``
@@ -312,15 +329,17 @@
     :raises: :py:exc:`khoros.errors.exceptions.MissingAuthDataError`
     """
     # Get the client ID
     if not _client_id:
         if _khoros_object and _khoros_object.bulk_data_settings.get('client_id'):
             _client_id = _khoros_object.bulk_data_settings.get('client_id')
         else:
-            raise errors.exceptions.MissingAuthDataError('A valid Client ID is required to utilize the Bulk Data API.')
+            _error_msg = 'A valid Client ID is required to utilize the Bulk Data API.'
+            logger.error(_error_msg)
+            raise errors.exceptions.MissingAuthDataError(_error_msg)
 
     # Get the Accept value depending on the export type
     if not _export_type:
         if _khoros_object and _khoros_object.bulk_data_settings.get('export_type'):
             _export_type = _khoros_object.bulk_data_settings.get('export_type')
         else:
             # Default to CSV export
```

### Comparing `khoros-5.2.2/khoros/core.py` & `khoros-5.3.0.dev1/khoros/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 :Module:            khoros.core
 :Synopsis:          Collection of core functions and tools to work with the Khoros Community APIs
 :Usage:             ``import khoros.core`` *(Imported by default in primary package)*
 :Example:           ``khoros = Khoros(helper='helper.yml')``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     02 Nov 2022
+:Modified Date:     06 Jun 2023
 """
 
 import sys
 import copy
 import logging
 import warnings
 
@@ -42,15 +42,15 @@
         'auth_type': 'session_auth'
     }
 
     # Define the function that initializes the object instance (i.e. instantiates the object)
     def __init__(self, defined_settings=None, community_url=None, tenant_id=None, community_name=None, auth_type=None,
                  session_auth=None, oauth2=None, sso=None, helper=None, env_variables=None, auto_connect=True,
                  use_community_name=False, prefer_json=True, debug_mode=False, skip_env_variables=False, empty=False,
-                 ssl_verify=None, bulk_data_settings=None):
+                 ssl_verify=None, bulk_data_settings=None, logging_level=None):
         """This method instantiates the core Khoros object.
 
         .. versionchanged:: 5.0.0
            Added support for the Bulk Data API.
 
         .. versionchanged:: 4.3.0
            Fixed an issue where the ``ssl_verify`` parameter was being mostly disregarded.
@@ -111,14 +111,28 @@
         :raises: :py:exc:`khoros.errors.exceptions.MissingAuthDataError`,
                  :py:exc:`khoros.errors.exceptions.CurrentlyUnsupportedError`,
                  :py:exc:`khoros.errors.exceptions.SessionAuthenticationError`
         """
         # Define the current version
         self.version = version.get_full_version()
 
+        # Establish logging
+        self.logging = logging
+        if logging_level:
+            logging_levels = {
+                'DEBUG': logging.DEBUG,
+                'INFO': logging.INFO,
+                'WARNING': logging.WARNING,
+                'ERROR': logging.ERROR,
+                'CRITICAL': logging.CRITICAL,
+            }
+            if logging_level.upper() in logging_levels:
+                self.logging.basicConfig(level=logging_levels.get(logging_level))
+                logger.info(f'The {logging_level.upper()} logging level has been enabled.')
+
         # Initialize the predefined settings dictionary if not passed to the class
         defined_settings = {} if not defined_settings else defined_settings
 
         # Initialize other dictionaries that will be used by the class object
         self.auth = {}
         self.bulk_data_settings = {}
         self.core = {}
@@ -191,14 +205,15 @@
             self.core_settings['ssl_verify'] = self._helper_settings.get('ssl_verify')
         elif ssl_verify is None and self.core_settings.get('ssl_verify') is None:
             self.core_settings['ssl_verify'] = True
 
         # Update the global variable if SSL Verify is explicitly disabled
         if self.core_settings.get('ssl_verify') is False:
             api.ssl_verify_disabled = True
+            logger.warn('SSL verification has been disabled for the core Khoros object.')
 
         # Add the Bulk Data API settings if applicable
         if bulk_data_settings is not None and isinstance(bulk_data_settings, dict):
             self.bulk_data_settings = bulk_data_settings
         elif 'connection' in self._helper_settings and 'bulk_data' in self._helper_settings['connection']:
             self.bulk_data_settings = self._helper_settings['connection']['bulk_data']
         for bulk_data_field in ['community_id', 'client_id', 'token', 'europe', 'base_url', 'export_type']:
@@ -249,17 +264,14 @@
                 error_msg = f"No data was found for the default '{auth_type}' authentication type."
                 logger.error(error_msg)
                 raise errors.exceptions.MissingAuthDataError(error_msg)
 
         # Capture the version information
         self.sys_version_info = tuple([i for i in sys.version_info])
 
-        # Establish logging
-        self.logging = logging
-
         # Validate the settings
         self._validate_base_url()
         self._define_url_settings()
 
         # Populate the khoros.core dictionary with core settings
         self._populate_core_settings()
 
@@ -445,14 +457,17 @@
             _defined = True if ('username' in self.core_settings.get('session_auth') and
                                 'password' in self.core_settings.get('session_auth')) else _defined
         return _defined
 
     def _connect_with_session_key(self):
         """This method establishes a connection to the Khoros environment using basic / session key authentication.
 
+        .. versionchanged:: 5.3.0
+           Added a logging message when the connection has been established.
+
         .. versionchanged:: 4.2.0
            General code improvements were made to avoid unnecessary :py:exc:`KeyError` exceptions.
 
         .. versionchanged:: 3.3.2
            Added logging for the :py:exc:`khoros.errors.exceptions.MissingAuthDataError` exception.
 
         :raises: :py:exc:`khoros.errors.exceptions.MissingAuthDataError`
@@ -465,30 +480,35 @@
 
         self.core_settings['session_auth']['session_key'] = auth.get_session_key(self)
         self.core_settings['auth_header'] = \
             auth.get_session_header(self.core_settings.get('session_auth').get('session_key'))
         self.auth['session_key'] = self.core_settings.get('session_auth').get('session_key')
         self.auth['header'] = self.core_settings.get('auth_header')
         self.auth['active'] = True
+        logger.info('The connection to the Khoros environment has been established successfully.')
 
     def _connect_with_lithium_token(self):
         """This method establishes a connection to the Khoros environment using SSO authentication.
 
+        .. versionchanged:: 5.3.0
+           Added a logging message when the connection has been established.
+
         .. versionadded:: 4.2.0
 
         :raises: :py:exc:`khoros.errors.exceptions.MissingAuthDataError`
         """
         if "sso.authentication_token" not in self.core_settings.get('sso'):
             raise errors.exceptions.MissingAuthDataError("SSO authentication requires a LithiumSSO token.")
 
         li_api_session_key = auth.get_sso_key(self)
         session_key = auth.get_session_header(li_api_session_key)
         self.auth['session_key'] = session_key
         self.auth['header'] = session_key
         self.auth['active'] = True
+        logger.info('The connection to the Khoros environment has been established successfully.')
 
     def _import_v1_class(self):
         """This method allows the :py:class:`khoros.core.Khoros.V1` inner class to be utilized in the
         core object.
 
         .. versionadded:: 3.0.0
         """
@@ -1698,14 +1718,39 @@
             :param board_url: The URL of the board to check
             :type board_url: str, None
             :returns: Boolean value indicating whether the board already exists
             :raises: :py:exc:`khoros.errors.exceptions.MissingRequiredDataError`
             """
             return structures_module.boards.board_exists(self.khoros_object, board_id, board_url)
 
+        def get_message_count(self, board_id):
+            """This method retrieves the total number of messages within a given board.
+
+            .. versionadded:: 5.3.0
+
+            :param board_id: The ID of the board to query
+            :type board_id: str
+            :returns: The number of messages within the node
+            """
+            return structures_module.boards.get_message_count(self.khoros_object, board_id)
+
+        def get_all_messages(self, board_id, fields=None):
+            """This function retrieves data for all messages within a given board.
+
+            .. versionadded:: 5.3.0
+
+            :param board_id: The ID of the board to query
+            :type board_id: str
+            :param fields: Specific fields to query if not all fields are needed (comma-separated string or iterable)
+            :type fields: str, tuple, list, set, None
+            :returns: A list containing a dictionary of data for each message within the board
+            :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+            """
+            return structures_module.boards.get_all_messages(self.khoros_object, board_id, fields)
+
     class BulkData(object):
         """This class includes methods for interacting with the Bulk Data API.
 
         .. versionadded:: 5.0.0
         """
         def __init__(self, khoros_object):
             """This method initializes the :py:class:`khoros.core.Khoros.Board` inner class object.
```

### Comparing `khoros-5.2.2/khoros/errors/__init__.py` & `khoros-5.3.0.dev1/khoros/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/errors/exceptions.py` & `khoros-5.3.0.dev1/khoros/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/errors/handlers.py` & `khoros-5.3.0.dev1/khoros/errors/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         error_found, error_details = _get_v2_error_from_json(json_error)
     if include_error_bool:
         return error_found, error_details
     return error_details
 
 
 def verify_core_object_present(khoros_object):
-    """This function verifies whether or not the core object was supposed and raises an exception if not.
+    """This function verifies whether the core object was supposed and raises an exception if not.
 
     .. versionchanged:: 5.0.0
        Removed the redundant return statement.
 
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros]
     :returns: None
```

### Comparing `khoros-5.2.2/khoros/errors/translations.py` & `khoros-5.3.0.dev1/khoros/errors/translations.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/liql.py` & `khoros-5.3.0.dev1/khoros/liql.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,17 @@
     return f"{core_dict['v2_base']}/search?q={query}"
 
 
 def perform_query(khoros_object, query_url=None, liql_query=None, return_json=True, verify_success=False,
                   allow_exceptions=True, verify=None, return_items=False):
     """This function performs a LiQL query using full Community API v2 URL containing the query."
 
+    .. versionchanged:: 5.3.0
+       Added error logging to correspond with the raised exceptions.
+
     .. versionchanged:: 5.0.0
        Two ``if`` statements have been merged.
 
     .. versionchanged:: 4.1.0
        The JSON response can now be reduced to just the returned items by passing ``return_items=True``.
 
     .. versionchanged:: 3.4.0
@@ -144,20 +147,20 @@
     :type query_url: str, None
     :param liql_query: The LiQL query to be performed, not yet embedded in the query URL
     :type liql_query: str, None
     :param return_json: Determines if the response should be returned in JSON format (``True`` by default)
     :type return_json: bool
     :param verify_success: Optionally check to confirm that the API query was successful (``False`` by default)
     :type verify_success: bool
-    :param allow_exceptions: Defines whether or not exceptions can be raised for responses returning errors
+    :param allow_exceptions: Defines whether exceptions can be raised for responses returning errors
 
                              .. caution:: This does not apply to exceptions for missing required data.
 
     :type allow_exceptions: bool
-    :param verify: Determines whether or not to verify the server's TLS certificate (``True`` by default)
+    :param verify: Determines whether to verify the server's TLS certificate (``True`` by default)
     :type verify: bool, None
     :param return_items: Reduces the JSON response to be only the list of items returned from the LiQL response
                          (``False`` by default)
 
                          .. note:: If an error response is returned then an empty list will be returned.
 
     :type return_items: bool
@@ -167,19 +170,22 @@
              :py:exc:`khoros.errors.exceptions.MissingRequiredDataError`
     """
     # Determine if TLS certificates should be verified during API calls
     verify = api.should_verify_tls(khoros_object) if verify is None else verify
 
     # Validate the LiQL query
     if not query_url and not liql_query:
-        raise errors.exceptions.MissingRequiredDataError("An API query URL or a raw LiQL query must be provided.")
+        error_msg = "An API query URL or a raw LiQL query must be provided."
+        logger.error(error_msg)
+        raise errors.exceptions.MissingRequiredDataError(error_msg)
     if liql_query:
         query_url = get_query_url(khoros_object.core, liql_query)
     if 'header' not in khoros_object.auth:
         error_msg = "Cannot perform the query as an authorization header is not configured."
+        logger.error(error_msg)
         raise errors.exceptions.MissingAuthDataError(error_msg)
 
     # Perform the API call and validate the data
     response = api.get_request_with_retries(query_url, return_json, auth_dict=khoros_object.auth, verify=verify)
     if verify_success and not api.query_successful(response):
         error_msg = errors.handlers.get_error_from_json(response, include_error_bool=False)[2]
         if allow_exceptions:
```

### Comparing `khoros-5.2.2/khoros/objects/__init__.py` & `khoros-5.3.0.dev1/khoros/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/albums.py` & `khoros-5.3.0.dev1/khoros/objects/albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/archives.py` & `khoros-5.3.0.dev1/khoros/objects/archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/attachments.py` & `khoros-5.3.0.dev1/khoros/objects/attachments.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/base.py` & `khoros-5.3.0.dev1/khoros/objects/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/labels.py` & `khoros-5.3.0.dev1/khoros/objects/labels.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/messages.py` & `khoros-5.3.0.dev1/khoros/objects/messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/roles.py` & `khoros-5.3.0.dev1/khoros/objects/roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/settings.py` & `khoros-5.3.0.dev1/khoros/objects/settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/subscriptions.py` & `khoros-5.3.0.dev1/khoros/objects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/tags.py` & `khoros-5.3.0.dev1/khoros/objects/tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/objects/users.py` & `khoros-5.3.0.dev1/khoros/objects/users.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/saml.py` & `khoros-5.3.0.dev1/khoros/saml.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/structures/__init__.py` & `khoros-5.3.0.dev1/khoros/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/structures/base.py` & `khoros-5.3.0.dev1/khoros/structures/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/structures/boards.py` & `khoros-5.3.0.dev1/khoros/structures/boards.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 """
 :Module:            khoros.structures.boards
 :Synopsis:          This module contains functions specific to boards within the Khoros Community platform
 :Usage:             ``from khoros.structures import boards``
 :Example:           ``board_url = boards.create(khoros_object, 'my-board', 'My Board', 'forum', return_url=True)``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     23 May 2022
+:Modified Date:     05 Jun 2023
 """
 
 import warnings
+from operator import itemgetter
 
-from .. import api, errors
+from .. import api, liql, errors
 from ..objects import users
 from ..utils import log_utils
 from . import base
 
 # Initialize the logger for this module
 logger = log_utils.initialize_logging(__name__)
 
@@ -501,11 +502,133 @@
 
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros]
     :param board_id: The ID of the board to check
     :type board_id: str, None
     :param board_url: The URL of the board to check
     :type board_url: str, None
-    :returns: Boolean value indicating whether or not the board already exists
+    :returns: Boolean value indicating whether the board already exists
     :raises: :py:exc:`khoros.errors.exceptions.MissingRequiredDataError`
     """
     return base.structure_exists(khoros_object, 'board', board_id, board_url)
+
+
+def get_message_count(khoros_object, board_id):
+    """This function retrieves the total number of messages within a given board.
+
+    .. versionadded:: 5.3.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :param board_id: The ID of the board to query
+    :type board_id: str
+    :returns: The number of messages within the node
+    """
+    query = f"SELECT count(*) FROM messages WHERE board.id = '{board_id}'"
+    message_count = khoros_object.query(query).get('data').get('count')
+    return message_count
+
+
+def get_all_messages(khoros_object, board_id, fields=None):
+    """This function retrieves data for all messages within a given board.
+
+    .. versionadded:: 5.3.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :param board_id: The ID of the board to query
+    :type board_id: str
+    :param fields: Specific fields to query if not all fields are needed (comma-separated string or iterable)
+    :type fields: str, tuple, list, set, None
+    :returns: A list containing a dictionary of data for each message within the board
+    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+    """
+    # Define the variable where the messages will be stored
+    messages = []
+
+    # Define the LiQL query to be performed
+    fields = '*' if not fields else fields
+    if not isinstance(fields, str):
+        fields = liql.parse_select_fields(fields)
+    query = f"SELECT {fields} FROM messages WHERE board.id = '{board_id}' ORDER BY last_publish_time DESC LIMIT 1000"
+
+    # Perform the first LiQL query and add to the master list
+    response, cursor = _perform_single_query(khoros_object, query, fields)
+    messages.extend(response)
+
+    # Continue looping as long as a cursor is present
+    while cursor:
+        response, cursor = _perform_single_query(khoros_object, query, fields, cursor)
+        messages.extend(response)
+
+    # Return the collected messages
+    return messages
+
+
+def _perform_single_query(khoros_object, query, fields=None, cursor=None):
+    """This function performs a single LiQL query with or without a cursor.
+
+    .. versionadded:: 5.3.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :param query: The LiQL query to be performed
+    :type query: str
+    :param fields: Specific fields used in the LiQL SELECT statement
+    :type fields: str, tuple, list, set, None
+    :param cursor: The cursor from the LiQL response (when present)
+    :type cursor: str, None
+    :returns: The response to the LiQL query and the cursor when applicable
+    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+    """
+    # Construct the entire LiQL query
+    cursor = '' if not cursor else liql.structure_cursor_clause(cursor)
+    query = f"{query} {cursor}" if cursor else query
+
+    # Perform the API call and retrieve the data
+    response = liql.perform_query(khoros_object, liql_query=query)
+    data = liql.get_returned_items(response)
+
+    # Get the cursor when present
+    cursor = None
+    if response.get('data').get('next_cursor'):
+        cursor = response['data'].get('next_cursor')
+
+    # Add missing columns to message data as needed
+    data = _add_missing_cols(data, fields)
+    try:
+        data = sorted(data, key=itemgetter(*tuple(data[0].keys())))
+    except KeyError as missing_key:
+        logger.error(f'Could not sort the message data because the \'{missing_key}\' key was missing.')
+
+    # Return the user data and cursor
+    return data, cursor
+
+
+def _add_missing_cols(msg_list, fields=None):
+    """This function adds columns (fields) that might be missing from a LiQL response containing messages.
+
+    .. versionadded:: 5.3.0
+
+    :param msg_list: The list of dictionaries containing message data
+    :type msg_list: list
+    :param fields: Specific fields used in the LiQL SELECT statement
+    :type fields: str, tuple, list, set, None
+    :returns: The same Liql response data with the required columns included
+    """
+    new_list = []
+    required_cols = ['type', 'id', 'view_href', 'subject', 'last_publish_time']
+
+    # Add any defined fields to the list of required columns
+    if fields and fields != '*':
+        parsed_fields = fields.split(',')
+        for field in parsed_fields:
+            if field not in required_cols:
+                required_cols.append(field)
+
+    # Loop through the messages and add any missing columns
+    for msg in msg_list:
+        for col in required_cols:
+            if col not in msg:
+                msg[col] = ''
+        new_list.append(msg)
+    return new_list
```

### Comparing `khoros-5.2.2/khoros/structures/categories.py` & `khoros-5.3.0.dev1/khoros/structures/categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/structures/communities.py` & `khoros-5.3.0.dev1/khoros/structures/communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/structures/grouphubs.py` & `khoros-5.3.0.dev1/khoros/structures/grouphubs.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/structures/nodes.py` & `khoros-5.3.0.dev1/khoros/structures/nodes.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/studio/base.py` & `khoros-5.3.0.dev1/khoros/studio/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def sdk_installed():
     """This function checks to see if the Lithium SDK is installed.
 
     .. versionadded:: 2.5.1
 
-    :returns: Boolean value indicating whether or not the Lithium SDK is installed
+    :returns: Boolean value indicating whether the Lithium SDK is installed
     """
     try:
         output = core_utils.run_cmd('li')
         is_installed = True if output['return_code'] == 0 else False
     except FileNotFoundError:
         is_installed = False
     return is_installed
@@ -42,19 +42,19 @@
         output = core_utils.decode_binary(output)
         if '(empty)' not in output:
             version = output.split('lithium-sdk@')[1].split(' ')[0]
     return version
 
 
 def node_installed():
-    """This function checks whether or not Node.js is installed.
+    """This function checks whether Node.js is installed.
 
     .. versionadded:: 2.5.1
 
-    :returns: Boolean value indicating whether or not Node.js is installed
+    :returns: Boolean value indicating whether Node.js is installed
     """
     node_version = get_node_version()
     return True if node_version else False
 
 
 def get_node_version():
     """This function identifies and returns the installed Node.js version.
@@ -69,19 +69,19 @@
             version = version[1:]
     except FileNotFoundError:
         version = None
     return version
 
 
 def npm_installed():
-    """This function checks whether or not npm is installed.
+    """This function checks whether npm is installed.
 
     .. versionadded:: 2.5.1
 
-    :returns: Boolean value indicating whether or not npm is installed
+    :returns: Boolean value indicating whether npm is installed
     """
     npm_version = get_npm_version()
     return True if npm_version else False
 
 
 def get_npm_version():
     """This function identifies and returns the installed npm version.
```

### Comparing `khoros-5.2.2/khoros/utils/core_utils.py` & `khoros-5.3.0.dev1/khoros/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/environment.py` & `khoros-5.3.0.dev1/khoros/utils/environment.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/helper.py` & `khoros-5.3.0.dev1/khoros/utils/helper.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/log_utils.py` & `khoros-5.3.0.dev1/khoros/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/resources.py` & `khoros-5.3.0.dev1/khoros/utils/tests/resources.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_albums.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_archives.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_board_creation.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_board_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_bulk_data.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_categories.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_communities.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_core_utils.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_error_handling.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_exceptions.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_grouphub_creation.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_grouphub_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_helper_file.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_helper_file.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_http_headers.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_library_import.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_library_import.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_liql.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_mentions.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_messages.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_node_id_extract.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_node_id_extract.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_roles.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_settings.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_ssl_verify.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_ssl_verify.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_studio.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_tags.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_users.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/tests/test_version.py` & `khoros-5.3.0.dev1/khoros/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/khoros/utils/version.py` & `khoros-5.3.0.dev1/khoros/utils/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 """
 :Module:            khoros.utils.version
 :Synopsis:          This simple script contains the package version
 :Usage:             ``from .utils import version``
 :Example:           ``__version__ = version.get_full_version()``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     23 May 2023
+:Modified Date:     02 Jun 2023
 """
 
 import json
 import urllib.request
 
 from . import log_utils
 
 # Define special and global variables
-__version__ = "5.2.2"
+__version__ = "5.3.0dev1"
 latest_version_reported = False
 logger = log_utils.initialize_logging(__name__)
 
 
 def get_full_version():
     """This function returns the current full version of the khoros package."""
     return __version__
```

### Comparing `khoros-5.2.2/khoros.egg-info/PKG-INFO` & `khoros-5.3.0.dev1/khoros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.2.2
+Version: 5.3.0.dev1
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.2.2 Summary: Useful tools and
-utilities to assist in managing a Khoros Communities (formerly Lithium)
+Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev1 Summary: Useful tools
+and utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
```

### Comparing `khoros-5.2.2/khoros.egg-info/SOURCES.txt` & `khoros-5.3.0.dev1/khoros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khoros-5.2.2/pyproject.toml` & `khoros-5.3.0.dev1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khoros"
-version = "5.2.2"
+version = "5.3.0dev1"
 description = "Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment."
 authors = ["Jeff Shurtliff <jeff.shurtliff@rsa.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `khoros-5.2.2/setup.py` & `khoros-5.3.0.dev1/setup.py`

 * *Files identical despite different names*

